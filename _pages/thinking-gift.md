---
layout: archive
title: "A Data-Centric View of VPR Generalization"
permalink: /thinking/gift/
author_profile: true
---

[< Go back to Thinking]({{ '/thinking/' | relative_url }})

Visual place recognition models are usually evaluated across diverse, unseen test sets. This makes generalization a central challenge. Previous work has often focused on architectural improvements, aiming to learn robust descriptors across changing environments. However, under limited experimental conditions, many practical explorations eventually become incremental modifications to existing models.

Thanks to conversations with my friend [Yudian Zheng](https://yudianzheng.github.io/), my perspective shifted: exposing a VPR model to more distinctive and diverse visual data may be at least as important as changing its architecture. We explored how to extract useful priors from large generative models, from Stable Diffusion to ControlNet. Eventually, we adopted conditional image generation to synthesize outdoor scenes under varying weather and illumination conditions. By fine-tuning from these images, VPR models can acquire descriptors better aligned with real-world appearance changes.

The results behind GIFT are encouraging. It suggest that generative models contain discriminative knowledge for VPR. However, because they are trained for generation, their inference is not explicitly optimized for recognition. Fine-tuning a large generative model for VPR seems an interesting thing.
