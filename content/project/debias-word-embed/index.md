---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Debiasing Word Embeddings"
summary: "Mini-project that looks at potential bias in pre-trained word embeddings and methods on how to remove such bias."
authors: [Ayan Majumdar]
tags: ["Data Science", "NLP", "Fairness"]
categories: []
date: 2020-09-03T12:39:23+01:00

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: "Image courtesy [Salesforce](https://blog.einstein.ai/double-hard-debias-tailoring-word-embeddings-for-gender-bias-mitigation/)"
  focal_point: ""
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: "https://github.com/ayanmaj92/Coursera_Sequential_Models/blob/master/Sequential_Model/Week2/Assignments/Operations%2Bon%2Bword%2Bvectors%2B-%2Bv2.ipynb"
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
Ths mini-project aims to explore pre-trained Glove word embeddings for potential gender bias. We extract a gender-direction in the vector space of the word embeddings.
We then see how some words are incorrectly biased with respect to this gender direction, e.g. nurse is closer to female than male.

We attempt the debiasing methods offered [here](https://arxiv.org/abs/1607.06520). We show how such a simple debiasing method can reduce the bias.

<figure>
   <img src="featured_1.png" width="100%"></img>
    <figcaption><b>Bias neutralization method. Image courtesy <a href="https://www.coursera.org/learn/nlp-sequence-models">Coursera</a></b></figcaption>
</figure>

We also explore equalization, that aims to ensure that gender-specific words like actor and actress only differ with respect to the gender direction. This ensures that there is no indirect bias, e.g. actress is closer to babysit than actor, even though we may neutralize the bias that might be present in babysit.

<figure>
   <img src="featured_2.png" width="100%"></img>
    <figcaption><b>Bias equalization method. Image courtesy <a href="https://www.coursera.org/learn/nlp-sequence-models">Coursera</a></b></figcaption>
</figure>

**This project was completed as part of the Coursera course on Sequential Models.**
