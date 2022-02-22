---
layout: post
title:  Language modeling for improving maintenance services for medical devices
excerpt: "The goal of this project is to assist service engineers during remote maintenance activities of medical systems. When a system exhibits a problem, service engineers first try to diagnose the problem remotely and then decide the appropriate repair action(s) to take in order to remedy the problem."
modified: 11/07/2021, 10:35:24
tags: [Deep Learning, Natural Language Processing, Predictive Maintenance]
comments: false
category: mscfinished
---

The goal of this project is to assist service engineers during remote maintenance activities of medical systems. When a system exhibits a problem, service engineers first try to diagnose the problem remotely and then decide the appropriate repair action(s) to take in order to remedy the problem. In more complicated problems, the repair actions frequently include replacing one or more parts of the system.
 
While troubleshooting, service engineers use various tools that rely on Natural Language Processing techniques to analyze a vast amount of natural language data, such as machine log files. Log files are produced in huge amounts by software components, and salient information may be hard to find in such an amount of data. Being able to compress and encode long sequences of log data may help in providing the target learning algorithm with as much information as possible, and would avoid restrictions on the number and type of log lines to analyze, which may lead to unwanted bias.
 
Neural language modeling has been applied to compress and encode log files [1], in the attempt to overcome limitations posed by heuristic-based approaches. These, in fact, require great effort in design and adaptation and often work only for specialized cases. Attempts to apply state-of-the-art language modeling techniques, i.e., Transformers-based architecture, tackle mostly the anomaly detection task [2, 3]. Such previous attempts, however, relied on considerably short sequences of embeddings, constrained by structural properties of Transformer architectures. The application of techniques capable of handling longer input sequences, e.g., Longformers [4], is still to be investigated, especially their limitations in sequence length, and their integration with additional information coming from other sources (e.g., technical documents, maintenance service records etc.).

[1] S. Thaler, V. Menkovski and M. Petkovic, "Towards a neural language model for signature extraction from forensic logs," 2017 5th International Symposium on Digital Forensic and Security (ISDFS)

[2] Shaohan Huang, Yi Liu, Carol Fung, Rong He, Yining Zhao, Hailong Yang, Zhongzhi Luan, "HitAnomaly: Hierarchical Transformers for Anomaly Detection in System Log", 2020 IEEE Transactions on Network and Service Management

[3] Log representation as an interface for log processing applications, [https://openreview.net/pdf?id=-5VpoDCExrU](https://openreview.net/pdf?id=-5VpoDCExrU)

[4] Iz Beltagy, Matthew E. Peters, Arman Cohan, "Longformer: The Long-Document Transformer", 2020
 

Supervisor: Vlado Menkovski, Milosh Stolikj

