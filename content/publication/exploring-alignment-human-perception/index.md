---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Do Invariances in Deep Neural Networks Align with Human Perception?"
authors: 
- Vedant Nanda
- admin
- Camila Kolling
- John P. Dickerson
- Krishna P. Gummadi
- Bradley C. Love
- Adrian Weller

date: 2023-06-26T15:48:21+01:00
doi: "https://doi.org/10.1609/aaai.v37i8.26112"

# Schedule page publish date (NOT publication's date).
publishDate: 2023-6-26T15:48:21+01:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "AAAI Conference on Artificial Intelligence 2023"
publication_short: "AAAI 2023"

abstract: "An evaluation criterion for safe and trustworthy deep learning is how well the invariances captured by representations of deep neural networks (DNNs) are shared with humans. We identify challenges in measuring these invariances. Prior works used gradient-based methods to generate identically represented inputs (IRIs), ie, inputs which have identical representations (on a given layer) of a neural network, and thus capture invariances of a given network. One necessary criterion for a network's invariances to align with human perception is for its IRIs look 'similar' to humans. Prior works, however, have mixed takeaways; some argue that later layers of DNNs do not learn human-like invariances yet others seem to indicate otherwise. We argue that the loss function used to generate IRIs can heavily affect takeaways about invariances of the network and is the primary reason for these conflicting findings. We propose an adversarial regularizer on the IRI generation loss that finds IRIs that make any model appear to have very little shared invariance with humans. Based on this evidence, we argue that there is scope for improving models to have human-like invariances, and further, to have meaningful comparisons between models one should use IRIs generated using the regularizer-free loss. We then conduct an in-depth investigation of how different components (eg architectures, training losses, data augmentations) of the deep learning pipeline contribute to learning models that have good alignment with humans. We find that architectures with residual connections trained using a (self-supervised) contrastive loss with l_p ball adversarial data augmentation tend to learn invariances that are most aligned with humans."

# Summary. An optional shortened abstract.
summary: ""

tags: [deep learning, explainability]
categories: []
featured: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_pdf: https://ojs.aaai.org/index.php/AAAI/article/view/26112/25884
url_code: github.com/nvedant07/Human-NN-Alignment
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
