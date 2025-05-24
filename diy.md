---
layout: default
title: DIY
permalink: /diy/
---

# DIY Projects

Here’s a collection of tutorials and creative experiments — from handmade decor to wedding crafts.

<div class="post-grid">
  {% for post in site.posts %}
    {% if post.categories contains "diy" %}
      <div class="post-card">
        <a href="{{ post.url }}">
          <img src="{{ post.featured_image }}" alt="{{ post.title }}" loading="lazy">
          <h3>{{ post.title }}</h3>
        </a>
        <p class="post-date">{{ post.date | date: "%B %d, %Y" }}</p>
      </div>
    {% endif %}
  {% endfor %}
</div>
