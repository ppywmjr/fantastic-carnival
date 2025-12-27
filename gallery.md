---
layout: page
title: Gallery
permalink: /gallery/
---

<style>
  .gallery-container {
    display: grid;
    /* This creates a grid with 3 columns on desktop, 1 on mobile */
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    grid-gap: 15px;
    margin-top: 20px;
  }

  .gallery-item {
    overflow: hidden;
    border-radius: 8px;
    box-shadow: 0 4px 6px rgba(0,0,0,0.1);
    transition: transform 0.3s ease;
  }

  .gallery-item:hover {
    transform: scale(1.05);
  }

  .gallery-item img {
    width: 100%;
    height: 200px;
    object-fit: cover; /* This crops images to fit the square perfectly */
    display: block;
  }
</style>

<div class="gallery-container">
  <div class="gallery-item">
    <img src="{{ site.baseurl }}/assets/images/cat-attack.jpeg" alt="Description 1">
  </div>
  <div class="gallery-item">
    <img src="{{ site.baseurl }}/assets/images/crow.jpeg" alt="Description 2">
  </div>
  <div class="gallery-item">
    <img src="{{ site.baseurl }}/assets/images/rainbow-kitten.jpeg" alt="Description 3">
  </div>
</div>
