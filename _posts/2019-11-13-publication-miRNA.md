---
layout: post
title: Detection of pre-microRNA with Convolutional Neural Networks
authors: Jorge Cordero, Vlado Menkovski, Jens Allmer
excerpt:   Jorge Cordero, Vlado Menkovski, Jens Allmer (2019) "Detection of pre-microRNA with Convolutional Neural Networks"
modified: 06/9/2019, 9:00:24
tags: [convolutional neural networks, miRNA]
comments: true
category: publication
---

**Authors: Jorge Cordero, Vlado Menkovski, Jens Allmer**

**Abstract** 
MicroRNAs (miRNAs) are small non-coding RNA sequences that have been implicated in many physiological processes. Furthermore, miRNAs have been shown to be important biomarkers for diseases and their mimics are tested as drug candidates. The experimental discovery of miRNAs is complicated because both miRNAs and their targets need to be expressed for the confirmation of functional interaction. This is difficult since miRNA expression is under spatiotemporal control. This has motivated the development of computational methods for miRNA detection. Such computational methods typically involve the characterization of candidate sequences with features designed by domain experts and the application of statistical or machine learning algorithms. While such features can successfully encode domain knowledge, feature engineering is a difficult and time-consuming task. Additionally, some engineered features pose excessive computational complexity that can hinder the large scale detection of miRNA. In contrast, advances of representation learning methods such as deep learning provide for automatic development of effective features directly from data. In this work, we propose a method that uses domain knowledge to create an efficient image representation of miRNA molecules encoding sequence, structure, and implicitly some thermodynamic information. We then use this low-level feature representation of the molecules to develop a hierarchical deep representation using a convolutional neural network model, which directly detects precursor miRNAs. With this method we achieve state-of-the-art performance on all previously used datasets. Additionally, detection is achieved in real time thereby overcoming the high computational cost for current pre-miRNA feature calculations such as p-value based ones. Finally, the encoding and modeling process opens possibilities for interpretability of the models’ behavior, which may lead to novel biological interpretations of miRNA genesis and targeting.

**[bioRxiv link](https://www.biorxiv.org/content/10.1101/840579v1)**

