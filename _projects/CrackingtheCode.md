---
layout: page
title: Cracking the Code - Machine Learning and Medical Diagnosis 
description: Biomedical Engineering Society (BMES) at UC San Diego
img: assets/img/MRI.jpg
importance: 1
category: Teaching
related_publications: 
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/MRI.jpg" title="Yes label" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

This project and codebase was created for a machine learning workshop for the Biomedical Engineering Society (BMES) at UC San Diego. Here, we go over the basics of image classification in MRI imaging.

## Data Selection 

Data for this project was taken from [Kaggle](https://www.kaggle.com/datasets/navoneel/brain-mri-images-for-brain-tumor-detection). In this set, we are given images comprised of yes and no labels.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/DataBrain.png" title="Yes label" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

## Training and Testing

We preprocess the data by extracting the RGB values of the images after resizing. From here, we perform K-Nearest Neighbors (KNN) over a wide range of neighbors using 5-fold cross-validation. Using this approach, we are able to obtain an accuracy of 77.49% at 73 nearest neighbors.

You can find the link to the repository [here](https://github.com/darintsui/Workshops/tree/main/Cracking%20the%20Code%20-%20Machine%20Learning%20and%20Medical%20Diagnosis) and slides [here](https://github.com/darintsui/Workshops/blob/main/Cracking%20the%20Code%20-%20Machine%20Learning%20and%20Medical%20Diagnosis/Cracking%20the%20Code%20Machine%20Learning%20and%20Medical%20Diagnosis.pdf).
