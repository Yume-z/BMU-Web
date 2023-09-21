---
title: 'VertMatch A Semi-supervised Framework for Vertebral Structure Detection in 3D Ultrasound Volume'
authors:
  - Zeng Hongye
  - admin
date: '2020-12-01T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2017-01-01T00:00:00Z'

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['3']

# Publication name and optional abbreviated publication name.
publication: 'arXiv'
publication_short: ''

abstract: Three-dimensional (3D) ultrasound imaging technique has been applied for scoliosis assessment, but current assessment method only uses coronal projection image and cannot illustrate the 3D deformity and vertebra rotation. The vertebra detection is essential to reveal 3D spine information, but the detection task is challenging due to complex data and limited annotations. We propose VertMatch, a two-step framework to detect vertebral structures in 3D ultrasound volume by utilizing unlabeled data in semi-supervised manner. The first step is to detect the possible positions of structures on transverse slice globally, and then the local patches are cropped based on detected positions. The second step is to distinguish whether the patches contain real vertebral structures and screen the predicted positions from the first step. VertMatch develops three novel components for semi-supervised learning, for position detection in the first step, (1) anatomical prior is used to screen pseudo labels generated from confidence threshold method; (2) multi-slice consistency is used to utilize more unlabeled data by inputting multiple adjacent slices; (3) for patch identification in the second step, the categories are rebalanced in each batch to solve imbalance problem. Experimental results demonstrate that VertMatch can detect vertebra accurately in ultrasound volume and outperforms state-of-the-art methods. VertMatch is also validated in clinical application on forty ultrasound scans, and it can be a promising approach for 3D assessment of scoliosis.


# Summary. An optional shortened abstract.
summary: 

tags:
  - 
featured: true

links:
#   - name: Custom Link
#     url: http://example.org
# url_pdf: http://arxiv.org/pdf/1512.04133v1
url_code: '#'
url_dataset: '#'
url_poster: '#'
url_project: ''
url_slides: ''
url_source: '#'
url_video: '#'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/s9CC2SKySJM)'
  focal_point: ''
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
  # - internal-project

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides:
---


