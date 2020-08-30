---
layout: project
type: project
image: images/p3.png
title: MNIST Autoencoder
permalink: projects/p3
# All dates must be YYYY-MM-DD format!
date: 2019-07-01
labels:
  - Python
  - Keras
  - Tensorflow
  - Deep Learning
  - MNIST
  - Autoencoder
  - GitHub
summary: A simple python script to learn from MNIST daatset and recreate or predict numbers from 0-9.
---

<img class="ui image" src="{{ site.baseurl }}/images/cotton-header.png">

MNIST AutoEncoder is an autoencoder which can be used to generate the popular MNIST dataset and we can use the result to enhance the original dataset. We will build an autoencoder from scratch in TensorFlow and generate the actual images from the MNIST dataset.

Autoencoder is a neural network tries to learn a particular feature of converting an input to an output data and generate back the input given the output. It includes two parts:

    encoder: which learns the features of the data or given answers
    decoder: which tries to generate the answers from the learnt features/ questions

This technique is widely used for a variety of situations such as generating new images, removing noise from images and many others.

You can find more about [MNIST AutoEncoder](https://github.com/dnabanita7/DeepLearningProject/blob/master/autoencoder.ipynb).
