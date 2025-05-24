---
layout: default
title: Blog
permalink: /blog/
---

# Blog

{% if site.posts.size > 0 %}
<div class="post-grid">
  {% for post in site.posts %}
    {% unless post.categories contains "diy" %}
      <div class="post-card">
        <a href="{{ post.url }}">
          <div class="img-wrapper">
            <img 
              src="{{ post.featured_image | default: '/assets/images/fallback.jpg' }}" 
              onerror="this.onerror=null;this.src='/assets/images/fallback.jpg';" 
              alt="{{ post.title }}" 
              loading="lazy">
          </div>
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
