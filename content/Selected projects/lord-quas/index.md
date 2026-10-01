---
title: "Fractional Brownian Motion on a 3D Reconstructed Shape"
date: 2026-03-30
draft: false
description: "a description"
tags: ["example", "tag"]
showAuthor: false
showDate: false
showReadingTime: false
showWordCount: false
showHero: false
featured_image: "content/Selected projects/lord-quas/lord_quas_noise_anim_0.gif"
---

<div style="display: flex; gap: 1rem; flex-wrap: wrap; width: 100%;">
  <img src="lord_quas_map_normal_0.png" alt="Normal map of the reconstructed shape" style="flex: 1 1 200px; min-width: 0; margin: 0;">
  <img src="featured.gif" alt="Animated noise on the surface, with diffuse shading" style="flex: 1 1 200px; min-width: 0; margin: 0;">
</div>

As part of my Master's project, I'm working on 3D reconstruction of shapes via neural signed distance functions (SDFs). These are useful for sphere tracing (stepping along a ray by spheres with radius determined by the field). The [**codebase**](https://github.com/Galaxeaaa/HotSpot/tree/main) I'm using provides a ready-to-go sphere tracer which they use to compute renders of the surface, normal maps and heatmaps of intersections with the surface. I used this sphere tracer to identify the surface of the neural field and add texture; Fractional Brownian Motion inspired by [**Inigo Quilez**](https://iquilezles.org/articles/fbm/). Points on the surface are perturbed and coloured according to the noise added, creating swirling patterns. Using normals obtained through autograd of the neural distance field, I add simple diffuse shading to improve the appearance of the 3D object. 

<!-- Final result:
![1](featured.gif) -->

<!-- 
Without diffuse shading:
![1](lord_quas_map_noise_vanilla.gif) -->

