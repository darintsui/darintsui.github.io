---
layout: page
title: >
  A Gentle Introduction to Image Classification
description: Institute of Electrical and Electronics Engineers (IEEE) @ UC San Diego
img: assets/img/MNIST.png
importance: 1
category: Teaching
related_publications: 
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/MNIST.png" title="MNIST Digits" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

This project and codebase was created for a deep learning workshop for the Institute of Electrical and Electronics Engineers (IEEE) @ UCSD. Here, we go over the basics of image classification using convolutional neural networks (CNN) on the MNIST dataset.

## Data Selection 

Data for this project was taken from [MNIST dataset](https://www.tensorflow.org/datasets/catalog/mnist). In this set, we are given images comprised of handwritten digits from 0 to 9.

## Training and Testing

We format the data by one-hot encoding the labels from 0-9. We then look to normalize our data by dividing the pixel data information by 255. From here, we split our data into train and testing sets, and train a basic CNN model while varying common parameters such as learning rate, batch size, number of epochs, and optimizer. Using this implementation, we are able to obtain an accuracy of 98.77%.

## Future Work

For a more thorough implementation of CNN models on a harder dataset, feel free to check out my implementation of AlexNet on plankton classification! 

You can find the link to the repository [here](https://github.com/darintsui/Workshops/tree/main/Gentle%20Introduction%20to%20Image%20Classification) and slides [here](https://github.com/darintsui/Workshops/blob/main/Gentle%20Introduction%20to%20Image%20Classification/Machine%20Learning%20A%20Gentle%20Introduction%20to%20Image%20Classification%20.pdf).
