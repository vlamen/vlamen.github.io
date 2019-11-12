---
layout: post
title: Optimizing performance of a localization model by transfer learning using a novel autoencoder-like architecture
excerpt: "Project of Christoforos Boukouvalas"
modified: 07/22/2017, 9:00:24
tags: [transfer learning, localization, image analysis, cnn, unet]
comments: true
category: mscfinished
---

Recent advances in deep learning (via deep neural networks with convolutional layers), have allowed for computer vision to approach the effectiveness of the human brain in many vision related tasks. There is however still room for improvement and optimizing the current considered state of the art architectures is not trivial. One reason being that the neural networks are “black boxes” as it is difficult to get insights on the operations executed within the deeper layers and on how they reach specific results. 

One example of a challenging computer vision task is Identifying the location of objects on images, when the images are noisy or with little structure.  A (deep network) localization model can be trained to perform this task with supervised learning.  The training efficiency (and the performance of the model) is dependent on the number of labeled images used during training – the larger the number, the better the training. It is also dependent on the initialization of the weights of model at the beginning of the training.

During this project I will be investigating whether the performance of a localization model can be improved by initializing the first layers of the model using transfer learning. Transfer learning allows us to re-use part of (or even the whole of) an already trained model in order to receive “knowledge” that has already been gained. In the context of my research I will be first training using a model (the “gaze model”) that is tasked with identifying the objects in the image using an architecture similar to an autoencoder. While an autoencoder is tasked with outputting an image by learning compressed representations of all of its features, the “gaze model” is only trying to output an image, in which the objects of interest are highlighted. This will force the “gaze model” to only learn the features of the image that are of interest to us.

