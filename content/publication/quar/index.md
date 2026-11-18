---
title: 'Test-Time Adaptation of Quantized ViTs via Single-Pass Quantizer-Aligned Recalibration'

authors:
  - admin
  - Young D. Kwon
  - Sung-Ju Lee

date: '2026-10-06T13:48:33Z'
doi: '10.48550/arXiv.2610.08358'

publication_types: ['preprints']
publication: 'arXiv preprint'
publication_short: 'arXiv preprint'

abstract: >-
  Quantizer-Aligned Recalibration (QuAR) improves the robustness of quantized
  vision transformers by correcting shifted activations before they enter
  frozen quantizers. It aligns running channel statistics with source
  calibration using a single forward pass, without backpropagation or model
  parameter changes. Experiments span low-bit inference, corruption benchmarks,
  continual streams, label shifts, and multiple architectures. The results
  connect improved predictions to restored quantizer code distributions while
  keeping latency and additional memory small.

summary: >-
  Single-pass recalibration for robust quantized vision transformers, without
  backpropagation or parameter updates.

tags:
  - On-device AI
  - Test-time adaptation
  - Quantization
  - Vision Transformers

featured: true

url_pdf: 'https://arxiv.org/pdf/2610.08358'
url_code: 'https://github.com/chahh9808/QuAR'
url_project: '/post/quar/'
links:
  - name: arXiv
    url: 'https://arxiv.org/abs/2610.08358'
---
