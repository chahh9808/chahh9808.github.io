---
title: 'Poster: Time-Efficient Sparse and Lightweight Adaptation for Real-Time Mobile Applications'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - admin
  - Taesik Gong
  - Sung-Ju Lee

# Author notes (optional)
author_notes:
  - 'Equal contribution'

date: '2024-06-3T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2024-05-01T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['poster-conference']

# Publication name and optional abbreviated publication name.
publication: "The 22nd ACM International Conference on Mobile Systems, Applications, and Services"
publication_short: "MobiSys '24"

abstract: When deployed in mobile scenarios, deep learning models often suffer from performance degradation due to domain shifts. Test-Time Adaptation (TTA) offers a viable solution, but current approaches face latency issues on resource-constrained mobile devices. We propose TESLA Time-Efficient Sparse and Lightweight Adaptation strategy for real-time mobile applications, which skips adaptation for specific batches to increase the inference sample rate. Our method balances model accuracy and inference speed by accumulating domain-informative samples from non-adapted batches and sparsely adapting them. Experiments on edge devices demonstrate competitive accuracy even with sparse adaptation rates, highlighting the effectiveness of our approach in real-time mobile applications. Our strategy can seamlessly integrate with existing lightweight adaptation and optimization algorithms, further accelerating inference across diverse mobile systems.

# Summary. An optional shortened abstract.
summary: We propose TESLA Time-Efficient Sparse and Lightweight Adaptation strategy for real-time mobile applications, which skips adaptation for specific batches to increase the inference sample rate. Our method balances model accuracy and inference speed by accumulating domain-informative samples from non-adapted batches and sparsely adapting them.

tags:
  - On-device AI
  - Efficient Learning
  - Domain Adaptation

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: ''
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# image:
#   caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
#   focal_point: ''
#   preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---

<!-- {{% callout note %}}
Click the _Cite_ button above to demo the feature to enable visitors to import publication metadata into their reference management software.
{{% /callout %}}

{{% callout note %}}
Create your slides in Markdown - click the _Slides_ button to check out the example.
{{% /callout %}}

Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/). -->
