---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Exploring Representational Alignment with Human Perception Using Identically Represented Inputs"
authors: 
- Vedant Nanda
- admin
- Camila Kolling
- John P. Dickerson
- Krishna P. Gummadi
- Bradley C. Love
- Adrian Weller

date: 2021-10-30T15:48:21+01:00
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: 2021-10-30T15:48:21+01:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["3"]

# Publication name and optional abbreviated publication name.
publication: "CoRR:2111.14726"
publication_short: ""

abstract: "We contribute to the study of the quality of learned representations. In many domains, an important evaluation criterion for safe and trustworthy deep learning is how well the invariances captured by representations of deep neural networks (DNNs) are shared with humans. We identify challenges in measuring these invariances. Prior works used gradient-based methods to generate identically represented inputs (IRIs), i.e., inputs which have similar representations (on a given layer) of a neural network. If these IRIs look similar to humans then a neural network's learned invariances are said to align with human perception. However, we show that prior studies on the alignment of invariances between DNNs and humans are `biased' by the specific loss function used to generate IRIs. We show how different loss functions can lead to different takeaways about a model's shared invariances with humans. We show that under an adversarial IRI generation process all models appear to have very little shared invariance with humans. We conduct an in-depth investigation of how different components of the deep learning pipeline contribute to learning models that have good alignment with human's invariances. We find that architectures with residual connections trained using a self-supervised contrastive loss with \ell_p ball adversarial data augmentation tend to learn the most human-like invariances."

# Summary. An optional shortened abstract.
summary: ""

tags: [deep learning]
categories: []
featured: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_pdf: https://arxiv.org/pdf/2111.14726.pdf
url_code:
url_dataset:
url_poster:
url_project:
url_slides:
url_source:
url_video:

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: "Surveys for human invariance"
  focal_point: ""
  preview_only: false

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
