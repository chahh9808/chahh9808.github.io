---
title: 'Later Is Better: Token Reduction for ViTs Under Distribution Shift'
summary: >-
  A training-free token-reduction schedule that improves robustness under
  distribution shift by concentrating removal in later layers.
date: '2026-10-06T04:54:06Z'

image:
  caption: 'Late-concentrated token reduction under distribution shift ([paper](https://arxiv.org/abs/2610.07758)).'

authors:
  - admin
  - Hyungjun Yoon
  - Sung-Ju Lee

tags:
  - Vision Transformers
  - Token Reduction
  - Distribution Shift
---

## Position

First author

## Project Goals & Works

1. Study how the depth of token removal affects vision-transformer robustness under distribution shift.
2. Use a one-parameter power-law schedule to preserve tokens in early layers and concentrate removal in later layers.
3. Match the compute budget of a uniform removal schedule without retraining or input-specific tuning.

## Key Results

1. On ImageNet-C at severity 5, improved DeiT-S with ToMe by 1.17 percentage points over uniform removal at matched compute, while using about 26% less compute than the unreduced model.
2. Demonstrated improvements across five token-reduction methods and nine vision-transformer backbones.
3. Combined the schedule with six test-time adaptation methods, with further evaluations on video and vision-language tasks.

## Links

- [Publication details](/publication/later-is-better/)
- [arXiv](https://arxiv.org/abs/2610.07758)
- [Paper PDF](https://arxiv.org/pdf/2610.07758)
- [Code](https://github.com/chahh9808/LaterIsBetter)
