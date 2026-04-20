---
title: 'SNAP: Low-Latency Test-Time Adaptation with Sparse Updates'
summary: "A sparse test-time adaptation framework that significantly reduces adaptation latency while preserving accuracy on edge devices"
date: 2025-10-01

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: ''

authors:
  - admin
  - Dong Min Kim
  - Hye Won Chung
  - Taesik Gong
  - Sung-Ju Lee

tags:
  - On-device AI
  - Test-time adaptation
  - Efficient Learning
  - Edge Intelligence
---

## Position

First author project in KAIST Mobile Intelligence & Interaction Lab

## Project Goals & Works

1. Designed SNAP, a sparse Test-Time Adaptation (TTA) framework for latency-sensitive edge applications.
2. Proposed Class and Domain Representative Memory (CnDRM) to select a compact and informative subset of target samples for adaptation.
3. Proposed Inference-only Batch-aware Memory Normalization (IoBMN) to align normalization statistics at inference time with minimal overhead.
4. Integrated SNAP with five state-of-the-art TTA methods and validated consistent speedups with limited accuracy loss.

## Key Results

1. Reduced adaptation latency by up to 93.12% compared with baseline TTA pipelines.
2. Maintained competitive performance with less than 3.3% accuracy drop across adaptation rates from 1% to 50%.
3. Demonstrated strong practicality for resource-constrained, real-time on-device inference scenarios.

## Links

- Website: https://miil.kaist.ac.kr/projects/snap
- arXiv: https://arxiv.org/abs/2511.15276
- Code: https://github.com/chahh9808/SNAP
