---
layout: default
title: Blog
permalink: /blog/
---

# Blog

Welcome to my creative journal! Here's what's new (minus the glue and scissors — those live on the [DIY page](/diy/)).

{% if site.posts.size > 0 %}
<div class="post-grid">
  {% for post in site.posts %}
    {% unless post.categories contains "diy" %}
      <div class="post-card">
        <a href="{{ post.url }}">
          <img src="{{ post.featured_image }}" alt="{{ post.title }}" loading="lazy">
          <h3>{{ post.title }}</h3>
        </a>
        <p class="post-date">{{ post.date | date: "%B %d, %Y" }}</p>
      </div>
    {% endunless %}
  {% endfor %}
</div>
{% else %}
<p>No blog posts yet — check back soon!</p>
{% endif %}
