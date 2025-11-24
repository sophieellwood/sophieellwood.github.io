---
title: "RGB-D Facial Reconstruction (Computer Vision final project)"
date: 2025-11-21
draft: false
description: "a description"
tags: ["example", "tag"]
showAuthor: false
showDate: false
showReadingTime: false
showWordCount: false
showHero: false
---

[Code](https://github.com/sophieellwood/Computer-Vision-Final-Project/tree/main?tab=readme-ov-file)

# RGB-D Facial Reconstruction under Occlusion

This project addresses the challenge of reconstructing occluded facial regions using RGB-depth images. A non-occluded reference image is used for registration and provides the visual form of the occluded region. This method is particularly relevant for applications with access to extensive databases, such as hospital systems for recognizing masked employees in secure areas.

### Tested Occlusions:

- Blue medical face mask
- Black sunglasses
- Pink sunglasses
- Scarf
- Hands shielding the face

The primary focus is on face masks and black sunglasses as they occlude distinct facial regions without deforming the face and present distinct colors against other facial features. We are primarily focused on classical computer vision techniques to improve theoretical understanding, but we have included some DL/ML methods in certain pipelines as alternatives to our naive techniques, like DBSCAN.
