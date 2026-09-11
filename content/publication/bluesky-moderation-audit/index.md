---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Characterizing Bluesky Content Moderation Service: From Automation of Service to Landscape of Harms"
authors:
- Pushpdeep Singh
- Sayeh Jarollahi
- admin
- Vabuk Pahari
- Abhijnan Chakraborty
- Krishna P. Gummadi
- Ingmar Weber
- Abhisek Dash

date: 2026-09-11T00:00:00+01:00
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: 2026-09-11T00:00:00+01:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "AAAI ICWSM 2027 (Accepted)"
publication_short: "ICWSM 2027"

abstract: "Empirical research on content moderation is fundamentally constrained by the opaque deployment of moderation systems on major social media platforms. To this end, the recent emergence of decentralized platforms with transparent, public moderation logs presents an unprecedented opportunity for independent audits. In this work, we leverage this architectural transparency to conduct the first large-scale audit of the default moderation system on Bluesky, the Bluesky Moderation Service (BMS). Analyzing its 10.6M moderation labels from 2025, we investigate three foundational aspects: (i) its mechanism (the degree of automation versus human oversight), (ii) its efficacy (accuracy in detecting harms), and (iii) its purpose (the landscape of harms it identifies). Our findings reveal a human-AI collaborative system where labels for sexual and graphic content are applied automatically in seconds, while nuanced and high stakes labels require more human oversight, taking hours or days. Through a manual annotation study, we find the BMS operates with high precision (0.837), but struggles with low recall (0.222), with our annotators identifying 4.5× more harmful content than the moderation system in a random sample. Finally, unsupervised clustering of the most frequently applied labeled posts uncovers detected harms ranging from hostility in discourse toward protected groups to the spread of sexually explicit and other graphic content. Our work offers a look into the operational realities of a deployed moderation system, providing a concrete data-driven foundation for designing more effective and transparent moderation systems."

# Summary. An optional shortened abstract.
summary: ""

tags: [content moderation, safety]
categories: []
featured: false

url_pdf: https://arxiv.org/pdf/2609.11373
url_code:
url_dataset:
url_poster:
url_project:
url_slides:
url_source:
url_video:

# Featured image
image:
  caption: "Bluesky Moderation Service: automation vs. human oversight labeling delay analysis"
  focal_point: "Center"
  preview_only: false

projects: []

slides: ""
---
