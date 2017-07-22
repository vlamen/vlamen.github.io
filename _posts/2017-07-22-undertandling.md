---
layout: post
title: Natural Language Processing topics with Understandling 
excerpt: "Project topic(s) on NLP ranging from topic classification, unsupervised parsing, unsupervised parsing with recursive autoencoders"
modified: 07/22/2017, 9:00:24
tags: [intro, beginner, jekyll, tutorial]
comments: true
category: mscproject
---

* Topic classification – there are two generic ways of looking at texts and finding out what they are about: text classification and topic modeling. The former is supervised and works well for few topics that are mutually exclusive, the latter is unsupervised and distils terms that best summarize the text. The goal of topic classification is to determine the topic of a text from a predefined large set of potential topics, if any at all. Topic modeling doesn’t adhere to a predefined set of topics and classification is futile if the set of classes is too high (more than 10).
* Fully unsupervised parsing – We currently manage to do deep parsing (constituent and dependency, but the former is of interest) in a semi-supervised way where we only need POS-tags (instead of fully annotated parse trees). There is an interesting though that using change-of-base and meta-language modeling can eliminate the need for POS-tagging. This would be the topic of this project.
* Fully unsupervised recursive autoencoders – Using the our parsing we manage to apply recursive auto encoders (Richard Socher’s way of doing NLP) in a supervised manner. A challenge yet open is to pre-train the RAEs with parsed data and aggregate beyond word-level into phrase/sentence level using the information captured in the parse tree.
