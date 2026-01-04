---
layout: page
title: Auto-labeling & VQA Fine-tuning Pipeline for E2E Autonomous Driving
description: Auto-labeling lanes/trajectories/actors from surround-view + LiDAR + HD maps and generating VQA fine-tuning JSONL
img: assets/img/etri.jpg
importance: 1
category: work
related_publications: false
---

## Overview
During my research internship, I developed an **auto-labeling tool** that extracts **lanes, trajectories, actors, and work-zones** from **surround-view cameras + LiDAR + HD maps**, and converts them into **VQA fine-tuning JSONL** for training vision-language models. :contentReference[oaicite:8]{index=8}

## What I Built
- **Auto-labeling tool (multi-modal)**
  - Extracted structured supervision signals:
    - lanes / trajectories / actors / work-zones
  - Inputs:
    - surround-view images
    - LiDAR
    - HD maps
  - Outputs:
    - VQA fine-tuning dataset in **JSONL** format :contentReference[oaicite:9]{index=9}

- **VLM-based scene understanding & decision outputs**
  - Used **vision-fine-tuned InternVL 3.0** and **GPT-4o/5 (API)** to produce:
    - scene-understanding
    - action-decision style outputs
  - Target: improving E2E autonomous driving reasoning quality :contentReference[oaicite:10]{index=10}

## My Role
- Built the end-to-end labeling-to-dataset pipeline
- Implemented dataset generation flow and VQA JSONL formatting
- Integrated VLM inference outputs into training-ready data generation :contentReference[oaicite:11]{index=11}

## Tech Stack
- Sensors / Mapping: Surround-view cameras, LiDAR, HD maps
- Dataset: VQA fine-tuning JSONL
- Models: InternVL 3.0 (vision fine-tuned), GPT-4o/5 (API) :contentReference[oaicite:12]{index=12}

## Media
Replace the images below with (1) dataset generation diagrams, (2) example labeled frames, (3) JSONL samples (blur sensitive info).

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/projects/autolabel-vqa/fig1.jpg" title="Pipeline overview: sensors → auto-labels → JSONL" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/projects/autolabel-vqa/fig2.jpg" title="Example frame: extracted lanes/actors" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/projects/autolabel-vqa/fig3.jpg" title="Example: VQA JSONL sample visualization" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Recommended visuals: label overlays, track/trajectory extraction, and JSONL schema screenshots.
</div>

## Key Takeaway
This project demonstrates my ability to:
- build scalable data pipelines for autonomy,
- bridge multi-modal perception into training data,
- and connect VLM outputs to E2E driving model development. :contentReference[oaicite:13]{index=13}
