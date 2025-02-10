---
title: "XR Prototypes"
excerpt: "As an XR researcher, I'm constantly exploring the possibilities of immersive technologies through the development of XR applications. My primary focus lies in crafting novel 3D interaction techniques aimed at elevating the user experience within these immersive environments. What you'll find inside is a selection of prototypes showcasing some of these explorations. These projects reflect my skills as a Unity developer, my innovative solutions for interaction design, and my ability to visually communicate complex concepts. The prototypes will provide a glimpse into the ongoing evolution of my work in shaping the future of XR interaction."
permalink: /portfolio/1-xr-prototypes
collection: portfolio
---

As an XR researcher, I'm constantly exploring the possibilities of immersive technologies through the development of XR applications. My primary focus lies in crafting novel 3D interaction techniques aimed at elevating the user experience within these immersive environments. What you'll find below is a selection of prototypes showcasing some of these explorations. These projects reflect my skills as a Unity developer, my innovative solutions for interaction design, and my ability to visually communicate complex concepts. I hope this provides a glimpse into the ongoing evolution of my work in shaping the future of XR interaction.

 <div class="row">
 {% for video in site.data.videos %}
   <div class="col-md-6">  <!-- Adjust col-md-* as needed -->
     <h2>{{ video.title }}</h2>
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