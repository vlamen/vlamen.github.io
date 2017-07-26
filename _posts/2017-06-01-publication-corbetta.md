---
layout: post
title: Weakly supervised training of deep convolutional neural networks for overhead pedestrian localization in depth fields 
authors: Alessandro Corbetta, Vlado Menkovski, Federico Toschi
excerpt: "Overhead depth map measurements capture sufficient amount of information to enable human experts to track pedestrians accurately. However, fully automating this process using image analysis algorithms can be challenging. Even though hand-crafted image analysis algorithms are successful in many common cases, they fail frequently when there are complex interactions of multiple objects in the image. Many of the assumptions underpinning the hand-crafted solutions do not hold in these cases and the multitude of ..."
modified: 06/9/2017, 9:00:24
tags: [computer vision, convolutional neural networks, deep learning, weak supervision]
comments: true
category: publication
---

**Authors: Alessandro Corbetta, Vlado Menkovski, Federico Toschi**

**Abstract** 
Overhead depth map measurements capture sufficient amount of information to enable human experts to track pedestrians accurately. However, fully automating this process using image analysis algorithms can be challenging. Even though hand-crafted image analysis algorithms are successful in many common cases, they fail frequently when there are complex interactions of multiple objects in the image. Many of the assumptions underpinning the hand-crafted solutions do not hold in these cases and the multitude of exceptions are hard to model precisely. Deep Learning (DL) algorithms, on the other hand, do not require hand crafted solutions and are the current state-of-the-art in object localization in images. However, they require exceeding amount of annotations to produce successful models. In the case of object localization these annotations are difficult and time consuming to produce. In this work we present an approach for developing pedestrian localization models using DL algorithms with efficient weak supervision from an expert. We circumvent the need for annotation of large corpus of data by annotating only small amount of patches and relying on synthetic data augmentation as a vehicle for injecting expert knowledge in the model training. This approach of weak supervision through expert selection of representative patches, suitable transformations and synthetic data augmentations enables us to successfully develop DL models for pedestrian localization efficiently.

**[arXiv preprint arXiv:1706.02850](https://arxiv.org/abs/1706.02850)**
