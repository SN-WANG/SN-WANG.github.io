---
title: "HyperFlowNet"
collection: portfolio
permalink: /portfolio/hyperflownet/
excerpt: "HyperFlowNet is a spatio-temporal neural operator for forecasting the transient evolution of velocity, pressure, and temperature fields in a high-pressure-difference hydrogen pipeline. It performs autoregressive prediction on a fixed irregular mesh and combines sliding-history attention, graph-aware interactions, rollout curriculum learning, and hard no-slip boundary projection."
tags:
  - Spatio-Temporal Neural Operator
  - Transient CFD
  - Autoregressive Rollout
  - Digital Twin
videos:
  - src: /files/portfolio/hyperflownet-fields.mp4
    poster: /images/portfolio/hyperflownet-fields.jpg
    label: "Velocity, pressure, and temperature predictions compared with CFD reference fields."
  - src: /files/portfolio/hyperflownet-vorticity.mp4
    poster: /images/portfolio/hyperflownet-vorticity.jpg
    label: "Axisymmetric digital-twin visualization of the predicted vorticity field."
---

HyperFlowNet predicts the transient evolution of physical fields in a high-pressure-difference hydrogen pipeline. The model operates autoregressively on a fixed irregular mesh and combines annealed sliding-history attention, graph-aware interactions, rollout curriculum learning, and hard no-slip boundary projection.

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
