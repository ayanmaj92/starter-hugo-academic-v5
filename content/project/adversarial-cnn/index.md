---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Adversarial Attacks and Defense for CNN"
summary: "The project explores CNN classification models and their vulnerability to various adversarial attacks. Also explores a defence mechanism for it."
authors: [Ayan Majumdar]
tags: ["Deep Learning", "Robustness", "Vision"]
categories: []
date: 2020-07-03T12:10:13+01:00

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: "https://github.com/ayanmaj92/ML_CyberSec/blob/master/Project2/Project_2_2571210_2571656_2576612.ipynb"
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
The project explores the vulnerability of deep CNN based model to adversarial attacks. Deep CNN models are used for image classification, here we analyze for the simple task of handwritten digit classification using MNIST dataset.

However, these models are not robust, and have been shown to be vulnerable to minor perturbations to the input, as are done to generate what we call adversarial attacks.
We explore two attack methods: Fast Gradient Sign Method (FGSM) and Momentum Iterative Method (MIM). We show that a model that gives accuracy of 96% on the original MNIST dataset fails miserably when dealing with such attacks. 
E.g. for FGMS the accuracy drops to around 30%, and it is just 0.6% for MIM!

<figure>
   <img src="featured_2.png" width="75%"></img> 
    <figcaption><b>Original label (Y-axis) to Predicted label (X-axis)</b></figcaption>
</figure>

Next, we explore a defence mechanism known as adversarial training, where we train the model with batches of such attacked images.
We train the model with samples of FGSM attacked images. 
We show that this drastically improves the robustness of the model for both attacks, for FGSM it goes to 93.4% whereas it improves to 77.6% for MIM.

<figure>
   <img src="featured_3.png" width="100%"></img> 
    <figcaption><b>Prediction probabilities for original model and defended model to attacked images</b></figcaption>
</figure>

**This project was completed as part of the Machine Learning in Cybersecurity course of Saarland University.**
