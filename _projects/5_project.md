---
layout: page
title: Woowa Bros. Robot Delivery Challenge
description: GPS-denied localization with 3D LiDAR + IMU and collision-risk-aware DWA planning using pedestrian motion estimation
img: assets/img/woowa.jpg
importance: 5
category: work
related_publications: false
---

## Overview
For the Woowa Bros. Robot Delivery Challenge, I focused on reliable navigation in complex environments by stabilizing **GPS-denied localization** and improving local planning safety with **collision-risk-aware DWA**. :contentReference[oaicite:29]{index=29}

## What I Did
- **GPS-denied localization stabilization**
  - Stabilized localization by fusing:
    - 3D LiDAR-based pose (against a prebuilt 3D map)
    - IMU measurements :contentReference[oaicite:30]{index=30}

- **Pedestrian motion estimation and safety-aware planning**
  - Estimated pedestrian **speed and direction** from **YOLOv5 + LiDAR** data.
  - Integrated **collision risk** into **DWA** to achieve safer local path planning. :contentReference[oaicite:31]{index=31}

## My Role
- Implemented the localization fusion approach for GPS-denied operation
- Built the pedestrian motion feature extraction and risk integration into DWA planning :contentReference[oaicite:32]{index=32}

## Tech Stack
- Localization: 3D LiDAR-based pose on prebuilt 3D map + IMU fusion
- Perception: YOLOv5 + LiDAR-based pedestrian motion estimation
- Local Planning: DWA with collision-risk augmentation :contentReference[oaicite:33]{index=33}

## Media
Replace placeholders with:
- localization plot (drift before/after)
- pedestrian motion vectors overlay
- DWA trajectory samples with risk scores

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/projects/woowa/fig1.jpg" title="GPS-denied localization fusion (3D LiDAR + IMU)" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/projects/woowa/fig2.jpg" title="Pedestrian motion estimation (YOLOv5 + LiDAR)" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/projects/woowa/fig3.jpg" title="Collision-risk-aware DWA planning" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Suggested visuals: localization robustness, motion estimation overlays, and safer trajectory selection via risk-aware DWA.
</div>

## Takeaway
This project demonstrates practical autonomy for real deployment conditions:
- robust localization when GPS is unreliable
- safe navigation among pedestrians via risk-aware planning :contentReference[oaicite:34]{index=34}
