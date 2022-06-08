---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Using VAE for Robustness"
summary: "Exploring potential use cases of variational autoencoders in the context of robustness of ML systems."
authors: [Ayan Majumdar]
tags: ["Deep Learning", "Generative Models", "Robustness", "Vision"]
categories: []
date: 2020-10-03T10:31:16+01:00

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: "Smart"
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: ""
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
The work explored various directions of robustness, from tackling out of sample data to adversarial attacks and calibrated outputs. 
We explore how we could use the variational autoencoder (VAE) model in such use-cases. 

We look in-depth at the VAE's behavior while tackling out-of-distribution (OOD) samples. 
We analyze the VAE latent distributional space to search for any possible signals we could use.
We also see how VAE reconstructions of the data could actually be used to detect OOD samples.

For adversarial samples, we again explore the VAE latent distributional space.
We additionally look at using the VAE to clean adversarial samples.
The idea is that the VAE would manage to map any adversarial sample back into the nearest point in the data manifold.

Finally, we explore if the VAE could be used to help a model make more calibrated decisions.

## A. Testing Classifier Response to Adversaries with VAE
Using FGSM and LBFGS adversarial attacks, we use the MNIST dataset to generate adversarial examples.
Utilizing the stochasticity of the VAE model, for each input image, we sample 10 different latent z representations, and correspondingly 10 different reconstructions.
Then, we see how consistent the predicted labels for these 10 images are for a trained classifier. Ideally, the classifier response should be consistent.
So, the number of different labels given to the set of 10 images should be 1.
- For the original MNIST images, this is the case. The classifier is almost always consistent.
- But, for adversarial images, the VAE reconstructions are *not always consistent*.
- So, for a lot more instances, the classifier predicts the different images having different labels.

This could potentially be used to detect anomalous data using VAEs.
![bar plot of adversarial predictions](diff_preds_adv_vae.png "Consistency of classifier prediction for multiple VAE reconstructions per original or adversarial image. Highest consistency for x-axis value 1.")

## B. Testing Classifier Calibration with VAE
Is there a relation between how well the VAE reconstructs an image and a classifier's confidence on the same?
So, would a VAE model reconstruct those images where a classifier would be more confident, in a much better way?
We test this in this experiment. Using MNIST data, for each image we use a trained classifier to check the confidence/probability strength of the classifier's prediction.
We also check the VAE reconstruction loss (standard pixel-wise MSE loss) for each image.
If the VAE can be used to test calibration, then low VAE reconstruction loss should correspond to high confidence in the classifier.
- We indeed see this. For images with high confidence, the VAE reports much lower loss.
- The loss slowly increases as the confidence reduces.
- But, we note that the signal here is not as strong.

Hence, using a VAE to test calibration would require further research.
![bar plot of calibration predictions](loss_conf_bins_20_calibration.png "Reconstruction loss vs classifier probability to test classifier calibration with VAE.")

**This project was done as a research assistant at the Max-Planck Institute for Software Systems.**
