---
title: >
  Cracking the Code - Machine Learning and Medical Diagnosis
summary: Provides a tutorial on image classification using MRI data, as well as an overview of machine learning in biomedical engineering.
tags:
  - Teaching
date: "2023-02-27"

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: MRI image with a brain tumor
  focal_point: Smart

links:
  - icon: github
    icon_pack: fab
    name: Code
    url: https://github.com/darintsui/Workshops/tree/main/Cracking%20the%20Code%20-%20Machine%20Learning%20and%20Medical%20Diagnosis
url_code: ''
url_pdf: ''
url_slides: 'Cracking the Code Machine Learning and Medical Diagnosis.pdf'
url_video: ''
share: false

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ''
---

This project and codebase was created for a machine learning workshop for the Biomedical Engineering Society (BMES) at UC San Diego. Here, we go over the basics of image classification in MRI imaging.

## Data Selection 

Data for this project was taken from [Kaggle](https://www.kaggle.com/datasets/navoneel/brain-mri-images-for-brain-tumor-detection). In this set, we are given images comprised of yes and no labels.

<p align="center">
<img src="yes.png" alt="Yes label" width="600"/>
</p>

## Training and Testing

We preprocess the data by extracting the RGB values of the images after resizing. From here, we perform K-Nearest Neighbors (KNN) over a wide range of neighbors using 5-fold cross-validation. Using this approach, we are able to obtain an accuracy of 77.49% at 73 nearest neighbors.
