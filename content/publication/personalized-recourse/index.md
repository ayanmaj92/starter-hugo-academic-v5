---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "From Universal to Individualized Actionability: Revisiting Personalization in Algorithmic Recourse"
authors:
- Lena Marie Budde
- admin
- Richard Uth
- Markus Langer
- Isabel Valera

date: 2026-06-01T00:00:00+01:00
doi: "https://doi.org/10.48550/arXiv.2604.08030"

# Schedule page publish date (NOT publication's date).
publishDate: 2026-06-01T00:00:00+01:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "ACM Conference on Fairness, Accountability, and Transparency, 2026"
publication_short: "ACM FAccT 2026"

abstract: "Algorithmic recourse aims to provide actionable recommendations that enable individuals to change unfavorable model outcomes, and prior work has extensively studied properties such as efficiency, robustness, and fairness. However, the role of personalization in recourse remains largely implicit and underexplored. While existing approaches incorporate elements of personalization through user interactions, they typically lack an explicit definition of personalization and do not systematically analyze its downstream effects on other recourse desiderata. In this paper, we formalize personalization as individual actionability, characterized along two dimensions: hard constraints that specify which features are individually actionable, and soft, individualized constraints that capture preferences over action values and costs. We operationalize these dimensions within the causal algorithmic recourse framework, adopting a pre-hoc user-prompting approach in which individuals express preferences via rankings or scores prior to the generation of any recourse recommendation. Through extensive empirical evaluation, we investigate how personalization interacts with key recourse desiderata, including validity, cost, and plausibility. Our results highlight important trade-offs: individual actionability constraints, particularly hard ones, can substantially degrade the plausibility and validity of recourse recommendations across amortized and non-amortized approaches. Notably, we also find that incorporating individual actionability can reveal disparities in the cost and plausibility of recourse actions across socio-demographic groups. These findings underscore the need for principled definitions, careful operationalization, and rigorous evaluation of personalization in algorithmic recourse."

# Summary. An optional shortened abstract.
summary: ""

tags: [explainability, fairness, recourse, causality]
categories: []
featured: false

url_pdf: https://arxiv.org/pdf/2604.08030
url_code:
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
  caption: ""
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---
