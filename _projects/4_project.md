---
layout: page
title: Outdoor Advertising Robot (Immersion Project)
description: Prediction-based dynamic obstacle avoidance with ByteTrack + Kalman and GUI-driven behavior-tree navigation
img: assets/img/immersion.jpg
importance: 4
category: work
related_publications: false
---

## Overview
I improved an outdoor autonomous robot stack by adding a **prediction-based dynamic obstacle avoidance** module and building a **GUI-linked behavior tree** for flexible navigation control. :contentReference[oaicite:22]{index=22}

## Key Contributions
- **Dynamic obstacle motion prediction**
  - Enhanced avoidance by predicting obstacle motion using **ByteTrack + Kalman filter**. :contentReference[oaicite:23]{index=23}

- **GUI-linked behavior tree navigation**
  - Developed a GUI-linked behavior tree to enable flexible, user-driven control over navigation behavior. :contentReference[oaicite:24]{index=24}

## Context / Role
In my role as an autonomous driving developer, I contributed to outdoor autonomy development and improved dynamic obstacle handling through prediction-based modules. :contentReference[oaicite:25]{index=25}

## Tech Stack
- Tracking & Prediction: ByteTrack, Kalman filter
- Decision & Control: Behavior Tree (GUI-linked)
- Outdoor autonomy stack integration (perception + navigation oriented) :contentReference[oaicite:26]{index=26}:contentReference[oaicite:27]{index=27}

## Media
Replace placeholders with:
- tracking visualization (ID + predicted trajectories)
- BT graph screenshots
- before/after avoidance behavior clips or images

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/projects/outdoor-robot/fig1.jpg" title="ByteTrack + Kalman: tracking & prediction" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/projects/outdoor-robot/fig2.jpg" title="GUI-linked behavior tree control" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/projects/outdoor-robot/fig3.jpg" title="Outdoor navigation run (qualitative)" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Recommended visuals: predicted obstacle motion, BT structure, and navigation trajectories in outdoor scenes.
</div>

## Takeaway
This project highlights my strengths in:
- integrating perception outputs into planning/control decisions,
- improving real-world robustness with motion prediction,
- and building human-in-the-loop tools (GUI + BT) for reliable autonomy. :contentReference[oaicite:28]{index=28}
