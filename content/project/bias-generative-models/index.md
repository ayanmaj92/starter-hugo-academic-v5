---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Bias in Generative Models"
summary: "This project explores the case for potential bias in generative models such as variational autoencoders. The project also briefly looks at ways to mitigate such bias."
authors: [Ayan Majumdar]
tags: ["Deep Learning", "Generative Models", "Fairness", "Vision"]
categories: []
date: 2020-11-01T10:44:48+01:00

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: "Smart"
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---
The project was carried out while I was a research assistant at the Max Planck Institute for Software Systems. The project explored the new direction of looking for potential bias in generative models. Models like variational autoencoders and GANs are becoming quite popular and also seeing deployment. The project aims to see if such models can exhibit any notion of bias. In particular, we explore variational autoenccoders and how the data that is generated or reconstructed by such models can be biased to certain demographics. 
The bias is attempted to be formally defined. The project also involves initial exploration for methods to de-bias such systems, e.g. using additional labels to supervise the training process of the generative models.
<p>
<b>This project was done in collaboration with Preethi Lahoti, Junaid Ali, Till Speicher and Krishna Gummadi.</b>
</p>
