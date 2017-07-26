---
layout: post
title: Towards a neural language model for signature extraction from forensic logs
excerpt: "Signature extraction is a critical preprocessing step in forensic log analysis because it enables sophisticated analysis techniques to be applied to logs. Currently, most signature extraction frameworks either use rule-based approaches or handcrafted algorithms. Rule-based systems are error-prone and require high maintenance effort. Hand-crafted algorithms use heuristics and tend to work well only for specialized use cases. In this paper we present a novel approach to extract signatures from forensic logs that is based on a neural language model. This language model learns to identify mutable and non-mutable parts in a log message. We use this information to extract signatures. Neural language models..."
modified: 28/4/2017, 9:00:24
tags: [computer security, recurrent neural networks, deep learning, neural language model]
comments: false
category: publication
---

**Abstract** 
Signature extraction is a critical preprocessing step in forensic log analysis because it enables sophisticated analysis techniques to be applied to logs. Currently, most signature extraction frameworks either use rule-based approaches or handcrafted algorithms. Rule-based systems are error-prone and require high maintenance effort. Hand-crafted algorithms use heuristics and tend to work well only for specialized use cases. In this paper we present a novel approach to extract signatures from forensic logs that is based on a neural language model. This language model learns to identify mutable and non-mutable parts in a log message. We use this information to extract signatures. Neural language models have shown to work extremely well for learning complex relationships in natural language text. We experimentally demonstrate that our model can detect which parts are mutable with an accuracy of 86.4%. We also show how extracted signatures can be used for clustering log lines.

**[IEEE Xplore](http://ieeexplore.ieee.org/document/7916497/)**
