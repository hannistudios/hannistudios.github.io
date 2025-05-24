---
layout: default
title: Blog
permalink: /blog/
---

# Blog

Welcome to my creative journal! Here's what's new:

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a><br>
      <small>{{ post.date | date: "%B %d, %Y" }}</small>
    </li>
  {% endfor %}
</ul>
