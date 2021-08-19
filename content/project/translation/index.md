---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Neural Machine Translation"
summary: "A mini-project that looks at the task of neural machine translation using sequential models and attention mechanism."
authors: [Ayan Majumdar]
tags: ["NLP", "Deep Learning"]
categories: []
date: 2020-07-01T13:51:40+01:00

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

url_code: "https://github.com/ayanmaj92/Coursera_Sequential_Models/blob/master/Sequential_Model/Week3/Assignments/Neural%2Bmachine%2Btranslation%2Bwith%2Battention%2B-%2Bv4.ipynb"
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
This mini-project explores the task of solving translating between two languages using sequential deep learning models.

For this project, we use a simpler task of translating between date formats.
We use a bi-directional LSTM model.
We also make use of a soft attention mechanism.
This allows the decoder model to learn which parts of the input to concentrate on for translating specific parts of the input.

<figure>
   <img src="featured_1.png" width="70%"></img>
    <figcaption><b>Visualizing attention weights</b></figcaption>
</figure>

For example, here we see that for outputting translated year, the model *attends* to the year part.
For the month, it *attends* to the month.

**This project was completed as part of the [Coursera course on Sequential Models](https://www.coursera.org/learn/nlp-sequence-models).**
