---
title: >
  Implementation and Optimization of Convolutional Neural Networks for Plankton Classification
summary: Implementation of AlexNet for plankton classification.
tags:
  - Deep Learning
date: "2023-04-05"

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Plankton classes
  focal_point: Smart

links:
  - icon: github
    icon_pack: fab
    name: Code
    url: https://github.com/darintsui/PlanktonClassification
url_code: ''
url_pdf: 'PlanktonCNN.pdf'
url_slides: ''
url_video: ''
share: false

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ''
---

In order to process the large amounts of image data collected by underwater imaging sensors, we evaluated the usage of convolutional neural networks to perform image classification. We preprocessed the image data and trained CNN models 121 different classes of plankton. 


## Data Selection 

Data for this project was taken from the [2014 National Data Science Bowl](https://www.kaggle.com/c/datasciencebowl). In this set, we are given images spanning 121 different classes of plankton. In addition, our dataset comes highly imbalanced. 

## Preprocessing and Optimization

Using the image data, we resize all images to be 48 x 48. We also nrmalize the RGB values of the images in accordance with their relative weight in grayscale. From here, we try several techniques to improve the accuracy of our classifier: varying learning rate, varying optimizer, implementing Leaky ReLU, implementing cross-validation, and augmenting data via affine transformation.

<p align="center">
<img src="parameters.png" alt="Default parameters used" width="400"/>
</p>

## Training and Testing

Using the data, we look to train and test our classifier using the AlexNet implementation from PyTorch. After hypertuning our parameters, we were able to obtain a classification accuracy of 74%.

<p align="center">
<img src="AlexNet.png" alt="AlexNet architecture" width="200"/>
</p>

## Acknowledgements

This group project was inspired by COGS 181: Neural Networks and Deep Learning, taught at UC San Diego under Dr. Zhuowen Tu.
