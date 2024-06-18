---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Scaling up Causal Algorithmic Recourse with CARMA"
event: "European Workshop on Algorithmic Fairness, 2024"
event_url: "https://2024.ewaf.org/home"
location: "Mainz, Germany"
address:
  street:
  city: Mainz
  region:
  postcode:
  country: Germany
summary: "Poster presentation highlighting our project on scaling up causal recourse by designing a novel amortized framework based on causal generative models and neural network based causal intervention predictors."
abstract: "Algorithms are increasingly used to automate large-scale decision-making processes, e.g., online platforms that make instant decisions in lending, hiring, and education. When such automated systems yield unfavorable decisions, it is imperative to allow for recourse by accompanying the instantaneous negative decisions with recommendations that can help affected individuals to overturn them. However, the practical challenges of providing algorithmic recourse in large-scale settings are not negligible: giving recourse recommendations that are actionable requires not only causal knowledge of the relationships between applicant features but also solving a complex combinatorial optimization problem for each rejected applicant. In this work, we introduce CARMA, a novel framework to generate causal recourse recommendations at scale. For practical settings with limited causal information, CARMA leverages pre-trained state-of-the-art causal generative models to find recourse recommendations. More importantly, CARMA addresses the scalability of finding these recommendations by casting the complex recourse optimization problem as a prediction task. By training a novel neural-network-based framework, CARMA efficiently solves the prediction task without requiring supervision for optimal recourse actions. Our extensive evaluations show that post-training, running inference on CARMA reliably amortizes causal recourse, generating optimal and instantaneous recommendations. CARMA exhibits flexibility, as its optimization is versatile with respect to the algorithmic decision-making and pre-trained causal generative models, provided their differentiability is ensured. Furthermore, we showcase CARMA in a case study, illustrating its ability to tailor causal recourse recommendations by readily incorporating population-level feature preferences based on factors such as difficulty or time needed. Finally, we discuss and highlight a potential use case of our amortized recourse framework for large-scale auditing of fairness in recourse."

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: 2024-07-02T17:00:00+01:00
#date_end: 2024-07-02T17:30:41+01:00
all_day: false

# Schedule page publish date (NOT talk date).
publishDate: 2024-06-16T17:32:41+01:00

authors: 
- admin
tags: ["Deep Learning", "Generative Models", "Explainability"]

# Is this a featured talk? (true/false)
featured: false

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

# Optional filename of your slides within your talk's folder or a URL.
url_slides:  

url_code:
url_pdf:
url_video: 

# Markdown Slides (optional).
#   Associate this talk with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: ["carma"]
---
