---
layout: page
title: Deep Mutual Distillation for Semi-Supervised Medical Image Segmentation
---
### Intro

Proposed a novel semi-supervised method called Deep Mutual Distillation for accurately segmenting the atria in cardiac MRI images, achieving state-of-the-art performance on benchmark datasets.

### Methods

<div style="text-align: center;">
   <img src="image/deep/1719507571425.png" alt="1719507571425" style="zoom:50%;" />
</div>
**Mutual Knowledge Distillation**

- Distill knowledge from each other
- Increase temperature above 1.0 to enhance entropy and exploration
- Utilize Dice loss to address class imbalance issues

### Results

<div style="text-align: center;">
  <img src="image/deep/1719507602936.png" alt="1719507602936" style="zoom: 25%;" />
  <img src="image/deep/1719507609101.png" alt="1719507609101" style="zoom:25%;" />
  <img src="image/deep/1719507617248.png" alt="1719507617248" style="zoom:25%;" />
</div>

### [Paper](https://link.springer.com/chapter/10.1007/978-3-031-43898-1_52)
