---
title: 'Test-Time Adaptation of Quantized ViTs via Single-Pass Quantizer-Aligned Recalibration'
summary: >-
  QuAR recalibrates quantized vision transformers in a single forward pass,
  improving robustness without backpropagation or parameter updates.
date: '2026-10-06T13:48:33Z'

image:
  caption: 'QuAR method overview ([paper](https://arxiv.org/abs/2610.08358)).'

authors:
  - admin
  - Young D. Kwon
  - Sung-Ju Lee

tags:
  - On-device AI
  - Test-time adaptation
  - Quantization
  - Vision Transformers
---

## Position

First author

## Project Goals & Works

1. Improve the robustness of quantized vision transformers under distribution shift while keeping the model and quantizers frozen.
2. Recalibrate activations at late-block quantizer inputs and the classifier input using running channel statistics and source calibration statistics.
3. Adapt within a single forward pass, without backpropagation, parameter updates, or storage of past samples.

## Key Results

1. On ImageNet-C at severity 5, improved ViT-B/16 accuracy over the strongest evaluated backpropagation-free baseline by 4.00 percentage points at W3A3 and 2.28 points at W8A8.
2. Used about 170 KB of state and reduced latency by at least 46% compared with the evaluated two-forward-pass methods.
3. Evaluated robustness across continual streams, label shifts, additional distribution shifts, and multiple architectures.

## Links

- [Publication details](/publication/quar/)
- [arXiv](https://arxiv.org/abs/2610.08358)
- [Paper PDF](https://arxiv.org/pdf/2610.08358)
- [Code](https://github.com/chahh9808/QuAR)
