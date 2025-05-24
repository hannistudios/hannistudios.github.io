---
layout: default
title: Welcome
---

# Hello!

## Recent Blog Posts

<div class="post-grid">
  {% for post in site.posts limit:3 %}
    <div class="post-card">
      <a href="{{ post.url }}">
        <img src="{{ post.featured_image }}" alt="{{ post.title }}">
        <h3>{{ post.title }}</h3>
      </a>
      <p class="post-date">{{ post.date | date: "%B %d, %Y" }}</p>
    </div>
  {% endfor %}
</div>

