---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "CARMA: A practical framework to generate recommendations for causal algorithmic recourse at scale"
authors:
- admin
- Isabel Valera


date: 2024-06-06T15:48:21+01:00
doi: "https://doi.org/10.1145/3630106.3659003"

# Schedule page publish date (NOT publication's date).
publishDate: 2024-06-06T15:48:21+01:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "ACM Conference on Fairness, Accountability, and Transparency, 2024"
publication_short: " ACM FAccT 2024"

abstract: "Algorithms are increasingly used to automate large-scale decision-making processes, e.g., online platforms that make instant decisions in lending, hiring, and education. When such automated systems yield unfavorable decisions, it is imperative to allow for recourse by accompanying the instantaneous negative decisions with recommendations that can help affected individuals to overturn them. However, the practical challenges of providing algorithmic recourse in large-scale settings are not negligible: giving recourse recommendations that are actionable requires not only causal knowledge of the relationships between applicant features but also solving a complex combinatorial optimization problem for each rejected applicant. In this work, we introduce CARMA, a novel framework to generate causal recourse recommendations at scale. For practical settings with limited causal information, CARMA leverages pre-trained state-of-the-art causal generative models to find recourse recommendations. More importantly, CARMA addresses the scalability of finding these recommendations by casting the complex recourse optimization problem as a prediction task. By training a novel neural-network-based framework, CARMA efficiently solves the prediction task without requiring supervision for optimal recourse actions. Our extensive evaluations show that post-training, running inference on CARMA reliably amortizes causal recourse, generating optimal and instantaneous recommendations. CARMA exhibits flexibility, as its optimization is versatile with respect to the algorithmic decision-making and pre-trained causal generative models, provided their differentiability is ensured. Furthermore, we showcase CARMA in a case study, illustrating its ability to tailor causal recourse recommendations by readily incorporating population-level feature preferences based on factors such as difficulty or time needed."

# Summary. An optional shortened abstract.
summary: ""

tags: [explainability]
categories: []
featured: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_pdf: https://dl.acm.org/doi/pdf/10.1145/3630106.3659003
url_code: https://github.com/ayanmaj92/carma-recourse/
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
  caption: "CARMA amortized causal recourse framework"
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
- carma

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---
