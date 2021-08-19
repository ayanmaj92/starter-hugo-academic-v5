---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Using VAE for Robustness"
summary: "Exploring potential use cases of variational autoencoders in the context of robustness of ML systems."
authors: [Ayan Majumdar]
tags: ["Deep Learning", "Generative Models", "Robustness", "Vision"]
categories: []
date: 2020-10-03T10:31:16+01:00

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
The work explored various directions of robustness, from tackling out of sample data to adversarial attacks and calibrated outputs. 
We explore how we could use the variational autoencoder (VAE) model in such use-cases. 

We look in-depth at the VAE's behavior while tackling out-of-distribution (OOD) samples. 
We analyze the VAE latent distributional space to search for any possible signals we could use.
We also see how VAE reconstructions of the data could actually be used to detect OOD samples.

For adversarial samples, we again explore the VAE latent distributional space.
We additionally look at using the VAE to clean adversarial samples.
The idea is that the VAE would manage to map any adversarial sample back into the nearest point in the data manifold.

Finally, we explore if the VAE could be used to help a model make more calibrated decisions.

**This project was done as a research assistant at the Max-Planck Institute for Software Systems.**
