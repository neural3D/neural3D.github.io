---
title: "Online Meeting and Discussion on InstantNGP"
excerpt_separator: "<!--more-->"
date: 2022-12-08T13:00:00-00:00
categories:
  - Blog
tags:
  - Meeting
  - Presentation
  - KTH
---
The second online meeting of the project gave the participants an introduction into Coordinate Based Hybrid Representation.
<!--more-->
KTH student Marcel Büsching introduced the topic by giving a presentation on Instant Neural Graphic Primitives (Müller er al., ACM ToG 2022), a newly proposed method to drastically decrease the training time for Neural Radiance Fields (Mildenhall et al., ECCV 2020).
The general idea for these coordinate-based hybrid representations is to partition the learned information between a multilayer perceptron (MLP) and a spatial data structure, such as voxels or in the case of the paper discussed, a hash map.
This makes it possible to reduce the size of the MLP used and thus reduce the training time.
