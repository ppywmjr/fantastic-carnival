---
layout: page
title: Gallery
permalink: /gallery/
---

<style>
  /* Keeping the same styling from before */
  .gallery-container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    grid-gap: 15px;
  }
  .gallery-item img {
    width: 100%;
    height: 200px;
    object-fit: cover;
    border-radius: 8px;
  }
</style>

<div class="gallery-container">
  {% for item in site.data.gallery %}
    <div class="gallery-item">
      <img src="{{ site.baseurl }}/{{ item.filename }}" alt="{{ item.alt }}">
    </div>
  {% endfor %}
</div>
