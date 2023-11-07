---
layout: page
title: >
  Convolutional Neural Networks for Plankton Classification
description: Implementation of AlexNet for plankton classification
img: assets/img/Plankton.png
importance: 1
category: Work
related_publications: 
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Plankton.png" title="Plankton familt" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

In order to process the large amounts of image data collected by underwater imaging sensors, we evaluated the usage of convolutional neural networks to perform image classification. We preprocessed the image data and trained CNN models 121 different classes of plankton. 


## Data Selection 

Data for this project was taken from the [2014 National Data Science Bowl](https://www.kaggle.com/c/datasciencebowl). In this set, we are given images spanning 121 different classes of plankton. In addition, our dataset comes highly imbalanced. 

## Preprocessing and Optimization

Using the image data, we resize all images to be 48 x 48. We also nrmalize the RGB values of the images in accordance with their relative weight in grayscale. From here, we try several techniques to improve the accuracy of our classifier: varying learning rate, varying optimizer, implementing Leaky ReLU, implementing cross-validation, and augmenting data via affine transformation.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/parameters.png" title="Default parameters used" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

## Training and Testing

Using the data, we look to train and test our classifier using the AlexNet implementation from PyTorch. After hypertuning our parameters, we were able to obtain a classification accuracy of 74%.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/AlexNet.png" title="AlexNet architecture" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

## Acknowledgements

This group project was inspired by COGS 181: Neural Networks and Deep Learning, taught at UC San Diego under Dr. Zhuowen Tu.

You can find the link to the repository [here](https://github.com/darintsui/PlanktonClassification) as well as the report <a href="..\..\assets\pdf\PlanktonCNN.pdf">here</a>.