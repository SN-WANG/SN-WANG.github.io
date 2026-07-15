---
title: "StructFieldNet"
collection: portfolio
permalink: /portfolio/structfieldnet/
excerpt: "StructFieldNet reconstructs full nodal von Mises stress fields for wing structures from grouped thickness variables and nodal coordinates on an unstructured finite-element mesh. It combines coordinate-design multiplicative lifting, Physics-Attention, and an SVD-initialized basis-plus-residual decoder to preserve global trends and localized stress hotspots."
tags:
  - Neural Operator
  - Stress Field Reconstruction
  - Unstructured Mesh
  - Physics-Attention
videos:
  - src: /files/portfolio/structfieldnet-comparison.mp4
    poster: /images/portfolio/structfieldnet-comparison.jpg
    label: "Reference, predicted, and absolute-error wing stress fields."
---

StructFieldNet reconstructs full nodal von Mises stress fields from grouped wing-thickness variables and reference coordinates on an unstructured finite-element mesh. Its coordinate-design multiplicative lifting, slice-space Physics-Attention, and SVD-initialized basis-plus-residual decoder preserve both global stress trends and localized hotspots.

<div class="portfolio-media-grid">
{% for video in page.videos %}
  <figure class="portfolio-media">
    <video controls muted loop playsinline preload="metadata" poster="{{ video.poster }}">
      <source src="{{ video.src }}" type="video/mp4">
      Your browser does not support embedded MP4 video.
    </video>
    <figcaption>{{ video.label }}</figcaption>
  </figure>
{% endfor %}
</div>
