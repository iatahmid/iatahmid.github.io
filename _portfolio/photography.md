---
title: "Photography"
excerpt: "These are the photos I took. <br/><img src='/images/500x300.png'>"
permalink: /portfolio/photography
collection: portfolio
---

<div class="row">
{% for item in site.data.gallery-photography %}
  <div class="col-md-4">
    <img src="{{ item.image }}" alt="{{ item.alt }}" class="img-fluid rounded">
    <p class="caption text-center">{{ item.caption }}</p>
  </div>
{% endfor %}
</div>