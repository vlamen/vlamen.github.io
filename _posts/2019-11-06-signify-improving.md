---
layout: post
title:  Improving automated visual quality control of 3D-printed products (Signify)
excerpt: "At Signify we are investigating and implementing automated visual quality control of our 3D-printed products in order to improve our quality control and to lower the cost of non-quality. A baseline method to obtain images and detect anomalies (defects) has already been developed, based on deep learning algorithms. We plan to simplify the setup for obtaining images, such that it will work faster and for a bigger variety of products. Therefore, our aim is to expand the current methods for fault detection, making them more robust, reliable, and more compatible to the images obtained with this new method."
modified: 11/13/2019, 10:35:24
tags: [deep learning]
comments: false
category: mscfinished
---

The goal of this assignment is to investigate and implement new methods for visual quality control, based on images of products after they have been manufactured in 3D printers. Our previous approaches used flatbed scanners to obtain images of the surface of one particular product. These images were then manually checked for possible defects, thus obtaining an image data set suitable for machine learning. Several deep learning methods were evaluated for the fault detection.

The previous approach involved challenges, such as:
 
 * Manual labelling is costly, so the dataset is relatively small
 * Defects are relatively rare, yielding an imbalanced dataset
 * The data is high-dimensional (images), but defects are typically only noticeable in a small area of the image

With a new data collection method, using cameras instead of a flatbed scanner, these challenges remain, and new ones arise:

 * Images of the same product show more variety; factors such as location, orientation, and lighting conditions may vary
 * 3D printing allows for customizability in products, previously unseen product shapes still need to be checked for defects in a reliable way

The suggested approach is to extend a previously tested approach  that poses the problem as anomaly detection, using Variational Autoencoders  to model normal, non-defective images, and detecting defects by finding anomalies to this model. In particular, the suggested approach is to utilize recent developments in the learning of “disentangled latent variables”    to obtain better representations of the available image data.

Signify will provide the means and methods to obtain the required image data and will take care of a suitable image dataset for developing and testing new visual quality control methods.

Supervision: Loek Tonnaer, Mike Holenderski, Vlado Menkovski

[1]  Tonnaer, Loek & Li, Jiapeng & Osin, Vladimir & Holenderski, Mike & Menkovski, Vlado. (2019). Anomaly Detection for Visual Quality Control of 3D-Printed Products. 1-8. 10.1109/IJCNN.2019.8852372.

[2]  Doersch, Carl. "Tutorial on variational autoencoders." arXiv preprint arXiv:1606.05908 (2016).

[3] Locatello, Francesco, et al. "Challenging Common Assumptions in the Unsupervised Learning of Disentangled Representations." International Conference on Machine Learning. 2019.

[4] Mathieu, Emile, et al. "Disentangling Disentanglement in Variational Autoencoders." International Conference on Machine Learning. 2019.

