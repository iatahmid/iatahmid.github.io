---
title: "Graphic Designs"
excerpt: "These are the graphic designs I created. <br/><img src='/images/500x300.png'>"
permalink: /portfolio/graphic-designs
collection: portfolio
---

<div class="row">
{% for item in site.data.gallery-designs %}
  <div class="col-md-4">
    <img src="{{ item.image }}" alt="{{ item.alt }}" class="img-fluid rounded">
    <p class="caption text-center">{{ item.caption }}</p>
  </div>
{% endfor %}
</div>