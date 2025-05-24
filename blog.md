---
layout: default
title: Blog
permalink: /blog/
---

# Blog

Welcome to my creative journal! Here's what's new (minus the glue and scissors — those live on the [DIY page](/diy/)):

<ul>
  {% for post in site.posts %}
    {% unless post.categories contains "diy" %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a><br>
        <small>{{ post.date | date: "%B %d, %Y" }}</small>
      </li>
    {% endunless %}
  {% endfor %}
</ul>
