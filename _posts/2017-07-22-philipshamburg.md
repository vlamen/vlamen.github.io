---
layout: post
title: Generative Neural Networks for reconstruction of medical images 
excerpt: "Medical Image analysis with generative neural networks at Philips Research in Hamburg"
modified: 07/22/2017, 9:00:24
tags: [gan, generative, neural networks, deep learning, medical image analysis]
comments: false
category: mscproject
---

Neural networks have demonstrated outstanding performance on a range of computer vision tasks such as image classification, segmentation and completion. Much of this success can be translated from the domain of 2d RGB photographs to the domain of single channel 2d Xray/US and 3d MR/CT medical images to locate, segment and quantify anatomical structures, artifacts, anomalies.
(a)    Image artifacts due to failures at the image acquisition, reconstruction, processing or storage stage can lead to missing or erroneous values in medical images at a pixel level. Generative neural networks have demonstrated powerful denoising and impainting results. We explore these techniques e.g. GAN, conditional GAN, denoising autoencoders to restore, fill and enhance medical images.
(b)    Convolutional architectures are often employed to leverage the number of parameters in 3d segmentation architectures by simultaneously encoding massive weight sharing and strict locality. However in most 3d modalities, the z-axis is different from the other two directions either in terms of resolution or in that it also contains acquisition time structure which suggests to restrict convolutions two 2 dimensions and to replace the convolution by a recurrent architecture (unidirectional, bidirectional, LSTM, etc.). We would like to analyse the trade-offs between these 2 settings.
 
Philips Research is a global organization that helps Philips introduce meaningful innovations that improve people’s lives. We provide technology options for innovations in the area of health and well-being, targeted at both developed and emerging markets. Positioned at the front-end of the innovation process, we work on everything from spotting trends and ideation to proof of concept and – where needed – first-of-a-kind product development.
 
Philips Research Hamburg [1] hosts 100 scientists improving medical image processing pipelines at various levels e.g. by advancing hardware, image reconstruction, image enhancement, image analysis and decision support for various modalities i.e. MR/CT/US/Xray. Machine learning and neural networks in particular are key technologies for the healthtec industry. Every year we host a dozen of master students and a couple of PhD students.
 
[1] [http://www.philips.com/a-w/research/locations/hamburg.html](http://www.philips.com/a-w/research/locations/hamburg.html)
