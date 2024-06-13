---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "CARMA: Causal Algorithmic Recourse with (Neural) Model-based Amortization"
summary: "We explore improving the practicality of providing causal recourse explanations through a novel neural network model-based automation framework."
authors: [Ayan Majumdar]
tags: ["Explainability", "Generative Models", "Deep Learning", "Causality"]
categories: []
date: 2024-06-10T10:44:48+01:00

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: "Causal recourse for algorithmic decision-making systems"
  focal_point: "Center"
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: "https://github.com/ayanmaj92/carma-recourse/"
url_pdf: "https://dl.acm.org/doi/pdf/10.1145/3630106.3659003"
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---
The project represents our recent [ACM FAccT 2024](https://facctconference.org/2024/index.html) paper.
Algorithmic recourse aims to provide explanations to automated algorithmic decision-making systems to enable end-users to understand what needs to be done to change the algorithm's prediction.
To this end, causal recourse showed that using the causal knowledge of the features is vital to ensuring the recommendations are actionable by people while being optimal in terms of cost of feature changes.
However, causal recourse has two major practical limitations: i) it requires perfect causal knowledge to compute counterfactual outcomes of its causal recommendations, ii) it needs to solve separate combinatorially complex optimization problems for each person seeking recourse.
Hence, for large-scale automated systems, e.g., online applications that provide instantaneous automated lending decisions or instantly filter out CVs in hiring, causal recourse cannot be directly applied.
In this work, we introduce CARMA, a practical framework that i) incorporates the power of the latest causal generative models with ii) neural networks that solve a novel amortized predictive formulation of the separate combinatorial problems.
Using this practical approach, we show that CARMA can help scale up causal recourse to enable instantaneous, actionable, and optimal recourse recommendation generation.

## A. Limitations of existing causal recourse techniques
For each individual with features $\mathbf{x}^F$ requesting recourse, causal algorithmic recourse finds the optimal action $\boldsymbol{a}^*$ solves the following optimization problem 
$$
\begin{align}
\boldsymbol{a}^* \in \underset{\boldsymbol{a} \in \mathcal{A}\left(\mathbf{x}^{\mathrm{F}}\right)}{\arg \min } \operatorname{cost}\left(\boldsymbol{a} ; \mathbf{x}^{\mathrm{F}}\right) \text { subj.to } h\left(\mathbf{x}^{\mathrm{CF}}\left(\boldsymbol{a}, \mathbf{x}^{\mathrm{F}}\right)\right)=1
\end{align}
$$
## B. Amortizing causal recourse optimization with CARMA

## C. CARMA provides recourse that is optimal and instant

## D. CARMA is flexible in using different generative models

## D. CARMA can incorporate population-level feature preferences
