---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Generating Counterfactuals for Causal Fairness"
summary: "Project that was conducted as part of my Master's thesis to explore the application of generative models to compute counterfactuals for fairness."
authors: [Ayan Majumdar]
tags: ["Deep Learning", "Generative Models", "Causality", "Fairness",]
categories: []
date: 2020-11-02T09:54:04+01:00

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: "Right"
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: ""
url_pdf: "../../talk/master-seminar/thesis_cs_msc_majumdar_ayan.pdf"
url_slides: "../../talk/master-seminar/master-thesis_presentation.pdf"
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---
Notions of causal fairness for algorithmic decision making systems crucially rely on estimating whether an individual (or a group of individuals) and their counterfactual individual (or groups of individuals) would receive the same decision(s). Central to this estimation is the ability to compute the features of the counterfactual individual, given the features of any individual. Recent works have proposed to apply deep generative models like GANs and VAEs over real-world datasets to compute counterfactual datasets at the level of both individuals and groups. In this paper, we explore the challenges with computing accurate counterfactuals, particularly over heterogenous tabular data that is often used in algorithmic decision making systems. We also investigate the implicit assumptions when applying deep generative models to compute counterfactual datasets.

<p>
<b>This project was done in collaboration with Preethi Lahoti, Junaid Ali, Till Speicher, Isabel Valera and Krishna Gummadi.</b>
</p>
