---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Can Foundation Models Moderate Online Content? Evaluating Instruction- vs. Example-Driven Policy Operationalization"
authors:
- admin
- Shounak Paul
- Pushpdeep Singh
- Ines Abdelaziz
- Sayeh Jarollahi
- Seungeon Lee
- Krishna P. Gummadi
- Ingmar Weber
- Abhisek Dash

date: 2026-09-01T00:00:00+01:00
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: 2026-09-01T00:00:00+01:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["3"]

# Publication name and optional abbreviated publication name.
publication: "arXiv preprint arXiv:2609.10410"
publication_short: "arXiv"

abstract: "The growing complexity of content moderation policies presents a critical challenge for their consistent operationalization. While foundation models possess the basic capabilities needed to confront this challenge, whether they can reliably moderate online content remains an unanswered question. In this paper, we systematically compare two competing paradigms for Vision-Language Model (VLM) guidance: an instruction-driven approach where models reason from policy precepts, and an example-driven approach where they generalize from prior precedents. We ground this investigation in ModerationBench, a new benchmark of 4,000 manually annotated, in-the-wild posts from the Bluesky platform. Our experiments reveal that foundation models can substantially outperform Bluesky's deployed moderation system, nearly tripling its F₁ score (0.60 vs. 0.22) on Random Posts in the benchmark, with both instruction- and example-driven paradigms achieving comparable peak effectiveness. Our findings thus chart a path toward reliable and adaptable policy operationalization at scale."

# Summary. An optional shortened abstract.
summary: ""

tags: [llm, vlm, content moderation, benchmark, fairness]
categories: []
featured: false

url_pdf: https://arxiv.org/pdf/2609.10410
url_code: https://github.com/ayanmaj92/moderation-bench
url_dataset:
url_poster:
url_project: https://moderation-bench.github.io/
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
projects:
- moderation-bench

# Slides (optional).
slides: ""
---
