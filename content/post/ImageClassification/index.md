---
title: >
  Machine Learning: A Gentle Introduction to Image Classification
summary: Provides a tutorial on convolutional neural networks (CNN) on the MNIST dataset.
tags:
  - Teaching
  - Deep Learning
date: "2023-05-14"

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: MNIST digits
  focal_point: Smart

links:
  - icon: github
    icon_pack: fab
    name: Code
    url: https://github.com/darintsui/Workshops/tree/main/Gentle%20Introduction%20to%20Image%20Classification
url_code: ''
url_pdf: ''
url_slides: 'Machine Learning A Gentle Introduction to Image Classification.pdf'
url_video: ''
share: false

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ''
---

This project and codebase was created for a deep learning workshop for the Institute of Electrical and Electronics Engineers (IEEE) @ UCSD. Here, we go over the basics of image classification using convolutional neural networks (CNN) on the MNIST dataset.

## Data Selection 

Data for this project was taken from [MNIST dataset](https://www.tensorflow.org/datasets/catalog/mnist). In this set, we are given images comprised of handwritten digits from 0 to 9.

## Training and Testing

We format the data by one-hot encoding the labels from 0-9. We then look to normalize our data by dividing the pixel data information by 255. From here, we split our data into train and testing sets, and train a basic CNN model while varying common parameters such as learning rate, batch size, number of epochs, and optimizer. Using this implementation, we are able to obtain an accuracy of 98.77%.

## Future Work

For a more thorough implementation of CNN models on a harder dataset, feel free to check out my implementation of AlexNet on plankton classification! 
