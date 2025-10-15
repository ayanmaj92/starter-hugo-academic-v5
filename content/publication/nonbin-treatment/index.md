---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "A Causal Framework to Measure and Mitigate Non-binary Treatment Discrimination"
authors:
- admin
- Deborah D. Kanubala
- Kavya Gupta
- Isabel Valera

author_notes:
- "Equal contribution"
- "Equal contribution"


date: 2025-03-28T15:48:21+01:00
doi: "https://doi.org/10.48550/arXiv.2503.22454"

# Schedule page publish date (NOT publication's date).
publishDate: 2025-03-28T15:48:21+01:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["3"]

# Publication name and optional abbreviated publication name.
publication: "Arxiv"
publication_short: "Arxiv"

abstract: "Fairness studies of algorithmic decision-making systems often simplify complex decision processes, such as bail or loan approvals, into binary classification tasks. However, these approaches overlook that such decisions are not inherently binary (e.g., approve or not approve bail or loan); they also involve non-binary treatment decisions (e.g., bail conditions or loan terms) that can influence the downstream outcomes (e.g., loan repayment or reoffending). In this paper, we argue that non-binary treatment decisions are integral to the decision process and controlled by decision-makers and, therefore, should be central to fairness analyses in algorithmic decision-making. We propose a causal framework that extends fairness analyses and explicitly distinguishes between decision-subjects' covariates and the treatment decisions. This specification allows decision-makers to use our framework to (i) measure treatment disparity and its downstream effects in historical data and, using counterfactual reasoning, (ii) mitigate the impact of past unfair treatment decisions when automating decision-making. We use our framework to empirically analyze four widely used loan approval datasets to reveal potential disparity in non-binary treatment decisions and their discriminatory impact on outcomes, highlighting the need to incorporate treatment decisions in fairness assessments. Moreover, by intervening in treatment decisions, we show that our framework effectively mitigates treatment discrimination from historical data to ensure fair risk score estimation and (non-binary) decision-making processes that benefit all stakeholders."

# Summary. An optional shortened abstract.
summary: ""

tags: [fairness]
categories: []
featured: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_pdf: https://arxiv.org/pdf/2503.22454
url_code: https://github.com/ayanmaj92/fair-nonbin-treatment
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
  caption: "Causal framework for studying non-binary treatment disparities and their effect on outcomes"
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
# projects:
# - carma

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---
