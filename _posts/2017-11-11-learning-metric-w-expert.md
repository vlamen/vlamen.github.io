---
layout: post
title: Learning efficiently from expert feedback on digital pathology images 
excerpt: "Metric learning on medical images with weak supervision"
modified: 11/12/2017, 10:09:00
tags: [metric learning, weak supervision, neural networks, deep learning, medical image analysis]
comments: false
category: mscproject
---

Deep Learning methods given enough annotated data have shown superior performance in many image analysis settings. However, in many domain such as medical image analysis annotations by domain expers (i.e. radiologist, pathologist) are exceedingly expensive to acquire. The typical workflow of these experts does not require that they annotate all regions of the image to full detail. Furthermore, ground truth is commonnly established by follow-up tests (such as molecular test on the specific region). Given this the annotations are usually very sparse and with significant noise. Rather than taking the usaual end-to-end learning approach in this project the goal is to develop a iterative learning approach that establish communication between the algorithm and the expert.

In this setup the algorithm proposes labelling of the given regions in a digital pathology image with tissue sub-types. The expert can then interact with the propsed regions by making corrections or confirmations that the algorithm needs to incorporate into it's learning process and propose up-dated solutions given the learnings.

The proposed direction for the project solution falls with-in the unsupervised and semi-supervised domain of machine learning. The solutions could build from work done on Siamese network [1], Triplet network [2] and diffusion maps [3] for metric learning, Variational autoencoders [4] and Ladder networks [5] for unsupervised and semi-supervised learning.

In this project there may be possibilities to collaborate with experts from medical image analysis and machine learning from TU/e, UvA and collaborate with industry partners. 


[1] [http://ieeexplore.ieee.org/abstract/document/1467314/figures](Chopra, Sumit, Raia Hadsell, and Yann LeCun. "Learning a similarity metric discriminatively, with application to face verification." Computer Vision and Pattern Recognition, 2005. CVPR 2005. IEEE Computer Society Conference on. Vol. 1. IEEE, 2005.)
[2] [https://link.springer.com/chapter/10.1007/978-3-319-24261-3_7](Hoffer, Elad, and Nir Ailon. "Deep metric learning using triplet network." International Workshop on Similarity-Based Pattern Recognition. Springer, Cham, 2015.)
[3] [http://www.sciencedirect.com/science/article/pii/S1063520306000546](Coifman, Ronald R., and Stéphane Lafon. "Diffusion maps." Applied and computational harmonic analysis 21.1 (2006): 5-30.)
[4] [https://arxiv.org/abs/1312.6114](Kingma, Diederik P., and Max Welling. "Auto-encoding variational bayes." arXiv preprint arXiv:1312.6114 (2013).)
[5] [http://papers.nips.cc/paper/5947-semi-supervised-learning-with-ladder-networks](Rasmus, Antti, et al. "Semi-supervised learning with ladder networks." Advances in Neural Information Processing Systems. 2015.)