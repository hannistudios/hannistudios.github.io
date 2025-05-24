---
layout: default
title: DIY
permalink: /diy/
---

# DIY Projects

Here’s a collection of hands-on tutorials and creative experiments I’ve shared — from handmade decor to wedding crafts.

<ul>
  {% for post in site.posts %}
    {% if post.categories contains "diy" %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a><br>
        <small>{{ post.date | date: "%B %d, %Y" }}</small>
      </li>
    {% endif %}
  {% endfor %}
</ul>
