---
layout: default
title: Blog
permalink: /blog/
---

# Blog

{% if site.posts.size > 0 %}
<div class="post-grid">
  {% for post in site.posts %}
    {% unless post.categories contains "diy" or post.categories contains "vintage" %}
      <div class="post-card">
        <div class="img-wrapper">
          <a href="{{ post.url }}">
            <img 
              src="{{ post.featured_image | default: '/assets/images/fallback.jpg' }}" 
              onerror="this.onerror=null;this.src='/assets/images/fallback.jpg';" 
              alt="{{ post.title }}" 
              loading="lazy">
          </a>
        </div>
        <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
        <p class="post-date">{{ post.date | date: "%B %d, %Y" }}</p>
      </div>
    {% endunless %}
  {% endfor %}
</div>
{% else %}
<p>No blog posts yet — check back soon!</p>
{% endif %}
