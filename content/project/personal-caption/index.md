---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Exploring Personalized Image Captioning"
summary: "This project explores personalization of generating image captions. We explore different architecture choices of Attend2u and also analyze personalization of the captions."
authors: [Ayan Majumdar]
tags: ["Vision", "NLP", "Deep Learning"]
categories: []
date: 2019-12-03T14:23:17+01:00

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: "Image courtesy [Attend2u](https://github.com/cesc-park/attend2u)"
  focal_point: ""
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: "https://github.com/ayanmaj92/attend2u"
url_pdf: "https://github.com/ayanmaj92/attend2u/blob/master/HLCV_Personalized_Caption_Project_Report.pdf"
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---
This work explores in detail the paper [Attend to You](https://arxiv.org/abs/1704.06485).
We look at the task of image captioning, that is generating textual description given any image.
However, here, we look at the task with an additional requirement of personalization.
So, a generated caption should reflect the style and vocabulary of particular users.

The model uses context memory cells, CNNs to generate captions using image features as well as particular user's context.
We base our analysis on a small subset of the InstaPIC dataset of the work.

<img src="featured_1.png"></img>

We explore different architecture choices, e.g. increasing memory capacity, increasing CNN channels and also dropout.
We analyze if changes in these choices affect the outcome.

For dropout, we explore using dropout at different locations of the model.

For metrics, we use BLEU-k, CIDEr, ROUGE_L, METEOR as used in the original work.
We see that increasing model capacity and also applying dropout manages to improve the model performance.
Of course, this needs to be further tested on the entire dataset with longer training durations.
This was not possible due to a lack of computing resources and time.

<figure>
<img src="featured_2.png" width="100%"></img>
<figcaption><b>Personalized captions by changing user context per image</b></figcaption>
</figure>

We also output different captions for the same image but changing the user's context to reflect the effect of personalization.
We see how changing the context manages to change the captions quite a bit for each image.
This shows how the model has actually learnt to use the user context and the image features both to generate meaningful but also personalized captions.

**This project was completed as part of the High-level Computer Vision course at Saarland University.**
