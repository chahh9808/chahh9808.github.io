---
title: 'SNAP: Low-Latency Test-Time Adaptation with Sparse Updates'

authors:
  - admin
  - Dong Min Kim
  - Hye Won Chung
  - Taesik Gong
  - Sung-Ju Lee

date: '2025-12-02T00:00:00Z'
doi: ''

publishDate: '2025-05-01T00:00:00Z'

publication_types: ['NeurIPS']

publication: "The Thirty-Ninth Annual Conference on Neural Information Processing Systems (NeurIPS '25)"
publication_short: "The Thirty-Ninth Annual Conference on Neural Information Processing Systems (NeurIPS '25)"

abstract: Test-Time Adaptation (TTA) adjusts models using unlabeled test data to handle dynamic distribution shifts. However, existing methods rely on frequent adaptation and high computational cost, making them unsuitable for resource-constrained edge environments. To address this, we propose SNAP, a sparse TTA framework that reduces adaptation frequency and data usage while preserving accuracy. SNAP maintains competitive accuracy even when adapting based on only 1% of the incoming data stream, demonstrating its robustness under infrequent updates. Our method introduces two key components. (i) Class and Domain Representative Memory (CnDRM), which identifies and stores a small set of samples that are representative of both class and domain characteristics to support efficient adaptation with limited data; and (ii) Inference-only Batch-aware Memory Normalization (IoBMN), which dynamically adjusts normalization statistics at inference time by leveraging these representative samples, enabling efficient alignment to shifting target domains. Integrated with five state-of-the-art TTA algorithms, SNAP reduces latency by up to 93.12%, while keeping the accuracy drop below 3.3%, even across adaptation rates ranging from 1% to 50%. This demonstrates its strong potential for practical use on edge devices serving latency-sensitive applications. The source code is available at https://github.com/chahh9808/SNAP.

summary: A sparse test-time adaptation framework that reduces adaptation latency while preserving accuracy on edge devices.

tags:
  - Unsupervised Domain adaptation
  - Test-time adaptation
  - Efficient AI

featured: true

url_pdf: ''
url_code: 'https://github.com/chahh9808/SNAP'
url_dataset: ''
url_poster: ''
url_project: 'https://miil.kaist.ac.kr/projects/snap/'
url_slides: ''
url_source: ''
url_video: ''

projects: []

slides: ""
---
