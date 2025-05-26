---
layout: default
title: DIY
permalink: /diy/
---

# DIY Projects

Here’s a collection of tutorials and creative experiments — from handmade decor to wedding crafts.

{% assign diy_posts = site.posts | where_exp: "post", "post.categories contains 'diy'" %}

{% if diy_posts.size > 0 %}
<div class="post-grid">
  {% for post in diy_posts %}
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
  {% endfor %}
</div>
{% else %}
<p>No DIY posts yet — but they’re coming soon!</p>
{% endif %}
