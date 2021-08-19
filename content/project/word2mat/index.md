---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Word2Mat: A New Word Representation"
summary: "This project explores a novel embedding technique for words into matrices instead of vectors. We explore this novel embedding method and how it could improve contextual sense."
authors: [Ayan Majumdar]
tags: ["NLP", "Deep Learning"]
categories: []
date: 2019-10-03T14:44:57+01:00

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

url_code: "https://github.com/ayanmaj92/word2mat-mlseminar18"
url_pdf: "https://github.com/ayanmaj92/word2mat-mlseminar18/blob/main/Word2Mat_Final_Report.docx.pdf"
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---
In this work, we explore how we could embed words into a new type of representation.
For NLP, words have been embedded into vectors (Word2Vec, Glove).
However, vector mathematics do not allow smartly recognizing context changes.
E.g. changing the order of words would not have any effect in the corresponding vector computations if we do dot products.

Instead, we attempt to embed the words into matrix form instead.
Matrix multiplication is non-commutative.
We hope that this new technique would make the representations themselves more context-aware.

We perform initial analysis for the same. We modify the Word2Vec model to allow for matrix embedding.
We further test for contextual sense by trying to predict the next token given the previous 2 tokens.

<figure>
<img src="featured_1.png"></img>
<figcaption><b>Analysis for contextual sense of embedding</b></figcaption>
</figure>

We see that matrix embedding can embed contextual sense.
E.g. for "wall street" we get "street" that signifies a very common trigram "wall street journal".
However, reversing the order and making it "street wall" simply predicts stop-words.
Note that if we use Word2Vec, both "wall street" and "street wall" would give same predictions, which is of course not optimal.

**This work was completed as part of the Machine Learning Seminar at Saarland University, supervised by Prof. [Dietrich Klakow](https://scholar.google.de/citations?user=_HtGYmoAAAAJ&hl=de).**
