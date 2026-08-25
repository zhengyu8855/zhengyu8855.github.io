---
layout: archive
title: "A Data-Centric View of VPR Generalization"
permalink: /thinking/gift/
author_profile: true
---

[< Go back to Thinking]({{ '/thinking/' | relative_url }})

Visual place recognition is usually trained on a large training dataset and evaluated across diverse, unseen test sets. This makes generalization a central challenge. Previous work has often focused on architectural improvements, aiming to learn descriptors that capture the statistical regularities of local structures and remain robust across changing environments. However, under limited experimental conditions, progress through architectural design alone can be incremental. Many practical explorations eventually become lightweight modifications to existing models.

Thanks to conversations with my friend [Yudian Zheng](https://yudianzheng.github.io/), my perspective shifted: exposing a VPR model to more distinctive and diverse visual data may be at least as important as changing its architecture. We explored how to extract useful priors from large generative models, from Stable Diffusion to ControlNet. Eventually, we adopted conditional image generation to synthesize outdoor scenes under varying weather and illumination conditions. By learning from these images, VPR models can acquire descriptors better aligned with real-world appearance changes.

The results behind GIFT are encouraging. They suggest that controlled synthetic data can be a practical route toward stronger VPR generalization, rather than relying solely on architectural changes. The performance of fine-tuning VPR models suggest that generative models contain discriminative knowledge. However, because they are trained for generation, their inference is not explicitly optimized for recognition. Fine-tuning a large generative model for VPR seems an interesting thing.
