---
title: "Graphic Designs"
excerpt: "Throughout my experiences with various organizations, I've had the opportunity to explore my passion for graphic design, primarily creating posters and banners for events and initiatives. I like playing with colors and perspectives to bring a minimalist and aesthetically pleasing approach to my work. This small collection showcases a few examples of these designs, reflecting my personal style and the specific needs of each organization."
permalink: /portfolio/2-graphic-designs
collection: portfolio
---

Throughout my experiences with various organizations, I've had the opportunity to explore my passion for graphic design, primarily creating posters and banners for events and initiatives. I like playing with colors and perspectives to bring a minimalist and aesthetically pleasing approach to my work. This small collection showcases a few examples of these designs, reflecting my personal style and the specific needs of each organization.

<div class="row">
{% for item in site.data.gallery-designs %}
  <div class="col-md-4">
    <img src="{{ item.image }}" alt="{{ item.alt }}" class="img-fluid rounded">
    <p class="caption text-center">{{ item.caption }}</p>
  </div>
{% endfor %}
</div>