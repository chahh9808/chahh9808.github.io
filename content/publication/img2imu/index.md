---
title: 'From Vision to Motion: Translating Large-Scale Knowledge for Data-Scarce IMU Applications'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Hyungjun Yoon
  - admin
  - Hoang C. Nguyen
  - Taesik Gong
  - Sung-Ju Lee

# Author notes (optional)
author_notes:
  - 'Equal contribution'

date: '2024-02-29T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2024-05-01T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['IEEE Transactions on Mobile Computing']

# Publication name and optional abbreviated publication name.
publication: "IEEE Transactions on Mobile Computing"
publication_short: "IEEE Transactions on Mobile Computing"

abstract: Pre-training representations acquired via self-supervised learning could achieve high accuracy on even tasks with small training data. Unlike in vision and natural language processing domains, pre-training for IMU-based applications is challenging, as there are few public datasets with sufficient size and diversity to learn generalizable representations. To overcome this problem, we propose IMG2IMU that adapts pre-trained representation from large-scale images to diverse IMU sensing tasks. We convert the sensor data into visually interpretable spectrograms for the model to utilize the knowledge gained from vision. We further present a sensor-aware pre-training method for images that enables models to acquire particularly impactful knowledge for IMU sensing applications. This involves using contrastive learning on our augmentation set customized for the properties of sensor data. Our evaluation with four different IMU sensing tasks shows that IMG2IMU outperforms the baselines pre-trained on sensor data by an average of 9.6%p F1-score, illustrating that vision knowledge can be usefully incorporated into IMU sensing applications where only limited training data is available.

# Summary. An optional shortened abstract.
summary: Pre-training representations acquired via self-supervised learning could achieve high accuracy on even tasks with small training data. Unlike in vision and natural language processing domains, pre-training for IMU-based applications is challenging, as there are few public datasets with sufficient size and diversity to learn generalizable representations. To overcome this problem, we propose IMG2IMU that adapts pre-trained representation from large-scale images to diverse IMU sensing tasks. We convert the sensor data into visually interpretable spectrograms for the model to utilize the knowledge gained from vision. We further present a sensor-aware pre-training method for images that enables models to acquire particularly impactful knowledge for IMU sensing applications. This involves using contrastive learning on our augmentation set customized for the properties of sensor data. Our evaluation with four different IMU sensing tasks shows that IMG2IMU outperforms the baselines pre-trained on sensor data by an average of 9.6%p F1-score, illustrating that vision knowledge can be usefully incorporated into IMU sensing applications where only limited training data is available.

tags:
  - Mobile sensing
  - Self-supervised learning
  - Contrastive learning

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
