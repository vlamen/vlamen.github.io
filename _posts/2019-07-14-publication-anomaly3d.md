---
layout: post
title: Anomaly detection for visual quality control of 3D-printed products
authors: Loek Tonnaer, Jiapeng Li, Vladimir Osin, Mike Holenderski, Vlado Menkovski
excerpt:  Tonnaer, L., Li, J., Osin, V., Holenderski, M., & Menkovski, V. (2019, July). Anomaly detection for visual quality control of 3D-printed products. In 2019 International Joint Conference on Neural Networks (IJCNN) (pp. 1-8). IEEE.
modified: 06/9/2019, 9:00:24
tags: [computer vision, convolutional neural networks, deep learning, annomaly detection]
comments: true
category: publication
---

**Authors: Loek Tonnaer, Jiapeng Li, Vladimir Osin, Mike Holenderski, Vlado Menkovski**

**Abstract** 
We present a method for detection of surface defects in images of 3D-printed products that enables automated visual quality control. The data characterising this problem is typically high-dimensional (high-resolution images), imbalanced (defects are relatively rare), and has few labelled examples. We approach these challenges by formulating the problem as probabilistic anomaly detection, where we use Variational Autoencoders (VAE) to estimate the probability density of non-faulty products. We train the VAE in an unsupervised manner on images of non-faulty products only. A successful model will then assign high likelihood to unseen images of non-faulty products, and lower likelihood to images displaying defects.

We test this method on anomaly detection scenarios using the MNIST dataset, as well as on images of 3D-printed products. The  demonstrated performance is related to the capability of the model to closely estimate the density distribution of the non-faulty (expected) data. For both datasets we present empirical results that the likelihood estimated with a convolutional VAE can separate the normal and anomalous data. Moreover we show how the reconstruction capabilities of VAEs are highly informative for human observers towards localising potential anomalies, which can aid the quality control process.

**[IEEE Xplore link](https://ieeexplore.ieee.org/abstract/document/8852372)**
