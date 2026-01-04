---
layout: page
title: Enhancing Diffusion-Based End-to-End Autonomous Driving with VLM
description: VLM-guided dynamic anchor sampling + trajectory re-ranking for safer and more diverse planning
img: assets/img/diffusion.jpg
importance: 2
category: work
related_publications: false
---

## Overview
I improved a diffusion-based end-to-end (E2E) autonomous driving pipeline by introducing **VLM-guided dynamic anchor sampling** for trajectory diversity and a **VLM-based Trajectory Scorer** for robust final trajectory selection. :contentReference[oaicite:2]{index=2}

## What I Did
- **VLM-guided dynamic anchor sampling**
  - Increased trajectory diversity and overall performance by dynamically sampling anchor trajectories with VLM guidance. :contentReference[oaicite:3]{index=3}
  - Switched to a **lightweight YOLO-based sampler** for real-time operation while maintaining comparable results. :contentReference[oaicite:4]{index=4}

- **VLM-based Trajectory Scorer (re-ranking)**
  - Built a trajectory re-ranking module that evaluates candidates using:
    - **Centerline alignment**
    - **Collision-avoidance metrics**
  - Improved final path selection by scoring and selecting the best candidate trajectory. :contentReference[oaicite:5]{index=5}

## My Role
Owner of the core algorithmic improvements:
- Designed the sampling + scoring architecture
- Implemented real-time-friendly sampling (YOLO-based)
- Integrated the re-ranking scorer into the E2E planning stack :contentReference[oaicite:6]{index=6}

## Tech Stack
- Deep Learning / E2E Driving: Diffusion-based planning pipeline
- Vision & Sampling: YOLO-based lightweight sampler
- Reasoning & Scoring: VLM-based candidate evaluation module :contentReference[oaicite:7]{index=7}

## Media
Below are placeholders. Replace them with your own screenshots (qualitative results, failure cases, ablations, etc.).

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/projects/diffusiondrive/fig1.jpg" title="Dynamic anchor sampling overview" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/projects/diffusiondrive/fig2.jpg" title="Trajectory re-ranking with VLM scorer" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/projects/diffusiondrive/fig3.jpg" title="Qualitative comparison (before/after)" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Example visuals: sampling diversity, collision-avoidance improvements, and selected trajectory comparisons.
</div>

## Notes
- This page is written to be readable to both research and engineering audiences.
- If you want, I can also generate a concise “portfolio card” summary (2–3 lines) for the main projects page.
