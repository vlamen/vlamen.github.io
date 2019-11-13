---
layout: post
title:  Semi-supervised Learning of Hierarchical Attributes (OLX)
excerpt: "Semi supervised learning of a hierarchical representation of image data"
modified: 11/13/2019, 10:35:24
tags: [deep learning]
comments: false
category: mscproject
---

OLX Group, part of Naspers, is a network of trading platforms present in more than 40 countries in over 50 languages. The OLX platform makes it easy to connect people to buy, sell or exchange used goods and services. Every month, more than 350 million people use it to find and sell cars, real estate, home appliances, musical instruments, consumer electronic goods and more. Every month 60+ million new listings are posted. 

#### Motivation
The images of the objects sold in the OLX platform can be classified according to their attribute such as type, brand, color, material, etc. To identify the characteristics of the objects, a wide range of labeled data is required to train a suitable classification model. Labeling large datasets can become time consuming, especially for describing the hierarchy of an object’s characteristics. 
Each of the sold objects in the platform has a set of images together with a small text description and a general category label. Our main question is: How can we extrapolate the information we have to create a semi-supervised or unsupervised method for learning a hierarchy of descriptive attributes?

![Hiarchical labels image](../../images/posts/hierarchical-labels.png)

Figure 1. Example tree of attribute hierarchy  

#### Objective
The general goal of this project is to devise a semi-supervised or unsupervised method for classification of object images based on the underlying hierarchical attributes that describe an object. Possible solutions can incorporate the textual description of a product to obtain a semantic meaning of the obtained hierarchy.
In particular, there is an increasing interest in exploring the use of embeddings with a certain geometry to represent the underlying structure of a dataset. Hyperbolic spaces act as the continuous generalization of the hierarchical structure of trees and have been used for recommender systems (Vinh, Tay, Zhang, Cong, & Li, 2018)  and (Chamberlain et al., 2019).
There is recent work on unsupervised methods based on variational autoencoders with a hyperbolic latent space that can capture the underlying hierarchical structure of a dataset (Mathieu, Lan, Maddison, Tomioka, & Teh, 2019).
A possible solution can incorporate the embeddings of images in the hyperbolic hierarchical space and couple them with attribute extraction from text (Ghani, Probst, Liu, Krema, & Fano, 2007). 

#### Available Data

~1 million object data consisting of text, image(s) and category (~3000 categories).

Public datasets such as ImageNet (J. Deng et al. 2009) and grocery store dataset (M. Klasson, C. Zhang, H. Kjellstrom, 2019) with hierarchical classes. 

##### Bibliography

[1] Chamberlain, B. P., Hardwick, S. R., Wardrope, D. R., Dzogang, F., Daolio, F., & Vargas, S. (2019). Scalable Hyperbolic Recommender Systems, (February). Retrieved from http://arxiv.org/abs/1902.08648

[2] Ghani, R., Probst, K., Liu, Y., Krema, M., & Fano, A. (2007). Text mining for product attribute extraction. ACM SIGKDD Explorations Newsletter, 8(1), 41–48. https://doi.org/10.1145/1147234.1147241

[3]Mathieu, E., Lan, C. Le, Maddison, C. J., Tomioka, R., & Teh, Y. W. (2019). Hierarchical Representations with Poincaré Variational Auto-Encoders. Retrieved from http://arxiv.org/abs/1901.06033

[4]Vinh, T. D. Q., Tay, Y., Zhang, S., Cong, G., & Li, X. (2018). Hyperbolic Recommender Systems. Retrieved from http://arxiv.org/abs/1809.01703

[5] Wang, W. E. I., Zheng, V. W., Yu, H. A. N., & Miao, C. (2019). A Survey of Zero-Shot Learning : Settings , Methods ,. Tist, 10(2).

[6] J. Deng, W. Dong, R. Socher, L. J. Li, K. Li, L. Fei-fei (2009). ImageNet: A Large-Scale Hierarchical Image Database. IEEE CCVPR. 

[7] M. Klasson, C. Zhang, H. Kjellstrom. (2019) A Hierarchical Grocery Store Image Dataset with Visual and Semantic Labels, IEEE WCACV.


