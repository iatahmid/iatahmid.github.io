---
title: "Photography"
excerpt: "Photography is more than just a hobby for me. It's a way of seeing and understanding the world. It's a language spoken through light, shadow, and perspective, allowing me to translate emotions and tell stories that words sometimes fail to convey. Here is a small collection of images from my journey of self-understanding, each representing a moment deeply etched into my memory."
permalink: /portfolio/photography
collection: portfolio
---

Photography is more than just a hobby for me. It's a way of seeing and understanding the world. It's a language spoken through light, shadow, and perspective, allowing me to translate emotions and tell stories that words sometimes fail to convey. Here is a small collection of images from my journey of self-understanding, each representing a moment deeply etched into my memory.

<div class="row">
{% for item in site.data.gallery-photography %}
  <div class="col-md-4">
    <img src="{{ item.image }}" alt="{{ item.alt }}" class="img-fluid rounded">
    <p class="caption text-center">{{ item.caption }}</p>
  </div>
{% endfor %}
</div>