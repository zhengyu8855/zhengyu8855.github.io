---
layout: archive
title: "Resources"
permalink: /resources/
author_profile: true
redirect_from:
  - /others/
---

## GIFT Dataset

[GIFT: A Generative Imagined Fine-Tuning Framework for Visual Place Recognition](https://ieeexplore.ieee.org/abstract/document/11464626/) (ICASSP 2026). We used  generated images to fine-tune VPR model, improving the recognition performance under changing environmental conditions.

The [GIFT repository](https://github.com/kuzhengyu/GIFT) provides the dataset used in the paper: approximately 140,000 images generated from three [GSV-Cities](https://github.com/amaralibey/gsv-cities) source cities under six conditions, including snow, fog, sun, night, rain, and overcast. 
![Examples of GIFT-generated views under varying environmental conditions](/images/resources/gift-generated-samples.png){: .align-center}
*Examples of generated views under varying environmental and illumination conditions.*

## SIAT Dataset

[Semantic-focused Patch Tokenizer with Multi-branch Mixer for Visual Place Recognition](https://ieeexplore.ieee.org/abstract/document/10610372) (ICRA 2024). We deployed our VPR method on a mobile robot and validated it on our campus. The [SIAT dataset](https://drive.google.com/file/d/1gLo_W5ByhQdHkX_qvfmawxusSPbVrX1h/view?usp=sharing) is available for download.

![SIAT dataset](/images/resources/icra-campus-vpr-testset.png){: .align-center}
*VPR deployment on a SIAT campus mobile robot. (a) Our small robot :\). (b) Recorded loop-closure trajectory, key frames and camera regions. (c)(d) Query and reference images of the same place under different appearances and viewpoints.*

