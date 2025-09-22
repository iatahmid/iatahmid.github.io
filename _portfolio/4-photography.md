---
title: "Photography"
excerpt: "Photography is more than just a hobby for me. It's a way of seeing and understanding the world. It's a language spoken through light, shadow, and perspective, allowing me to translate emotions and tell stories that words sometimes fail to convey. Here is a small collection of images from my journey of self-understanding, each representing a moment deeply etched into my memory. Please visit my Instagram page to find the most updated collection."
permalink: /portfolio/photography
collection: portfolio
gallery:
  - url: /images/photography/aurnil.jpeg         # optional: full-size image (for popup)
    image_path: /images/photography/aurnil.jpeg # required: the thumbnail shown on the page
    alt: "Waterfall in Shenandoah"
    title: "Shenandoah, 2024"                            # appears in the popup overlay
  - url: /images/photography/aurnil.jpeg
    image_path: /images/photography/aurnil.jpeg
    alt: "Foggy morning, Blacksburg"
    title: "Blacksburg, 2025"
  - url: /images/photography/aurnil.jpeg
    image_path: /images/photography/aurnil.jpeg
    alt: "Street scene, Dhaka"
    title: "Dhaka, 2023"
---

Photography is more than just a hobby for me. It's a way of seeing and understanding the world. It's a language spoken through light, shadow, and perspective, allowing me to translate emotions and tell stories that words sometimes fail to convey. Here is a small collection of images from my journey of self-understanding, each representing a moment deeply etched into my memory. Please visit my Instagram page to find the most updated collection.

{% include gallery layout="third" caption="Selected photographs." %}

<div class="row">
{% for item in site.data.gallery-photography %}
  <div class="col-md-4">
    <img src="{{ item.image }}" alt="{{ item.alt }}" class="img-fluid rounded">
    <p class="caption text-center">{{ item.caption }}</p>
  </div>
{% endfor %}
</div>