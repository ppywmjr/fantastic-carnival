---
layout: home
title: Welcome
---

## Hello World!

This is my new website built with **Jekyll** and hosted on **GitHub Pages**. 

I created this entire site without leaving my browser!

## Latest Blog Posts

<ul>
  {% for post in site.posts limit:3 %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <span style="color: #888;">({{ post.date | date: "%b %-d, %Y" }})</span>
      <p>{{ post.excerpt }}</p>
    </li>
  {% endfor %}
</ul>
