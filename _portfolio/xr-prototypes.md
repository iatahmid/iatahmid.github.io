---
title: "XR Prototypes"
excerpt: "These are the XR prototypes I created. <br/><img src='/images/500x300.png'>"
permalink: /portfolio/xr-prototypes
collection: portfolio
---

 <div class="row">
 {% for video in site.data.videos %}
   <div class="col-md-6">  <!-- Adjust col-md-* as needed -->
     <h3>{{ video.title }}</h3>
     <div class="video-container">  <!-- Add a container for aspect ratio -->
       {{ video.embed_code }}
     </div>
     <p>{{ video.description }}</p>
   </div>
 {% endfor %}
 </div>

 <style>
  .video-container {
    position: relative;
    padding-bottom: 56.25%; /* 16:9 aspect ratio (adjust if needed) */
    height: 0;
    overflow: hidden;
  }

  .video-container iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
  }
 </style>