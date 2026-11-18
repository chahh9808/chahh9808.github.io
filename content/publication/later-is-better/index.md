---
title: 'Later Is Better: Token Reduction for ViTs Under Distribution Shift'

authors:
  - admin
  - Hyungjun Yoon
  - Sung-Ju Lee

date: '2026-10-06T04:54:06Z'
doi: '10.48550/arXiv.2610.07758'

publication_types: ['preprints']
publication: 'arXiv preprint'
publication_short: 'arXiv preprint'

abstract: >-
  This work examines how the depth at which tokens are removed affects
  vision-transformer robustness under distribution shift. A one-parameter
  power-law schedule concentrates removal in later layers, improving
  out-of-distribution accuracy without increasing inference cost. Its gains
  persist when compute is matched, even with fewer final tokens. Experiments
  cover different reduction methods, backbones, corruptions, additional shift
  benchmarks, video, vision-language tasks, and test-time adaptation methods.
  The findings associate early removal with errors propagating through more
  remaining layers and support a shared schedule without input-specific tuning.

summary: >-
  A training-free token-reduction schedule that improves robustness under
  distribution shift by concentrating removal in later layers.

tags:
  - Vision Transformers
  - Token Reduction
  - Distribution Shift

featured: true

url_pdf: 'https://arxiv.org/pdf/2610.07758'
url_code: 'https://github.com/chahh9808/LaterIsBetter'
url_project: '/post/later-is-better/'
links:
  - name: arXiv
    url: 'https://arxiv.org/abs/2610.07758'
---
