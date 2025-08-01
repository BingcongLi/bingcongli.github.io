---
permalink: /
title: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
Welcome, it's a pleasure to connect with you! I'm Bingcong Li, a postdoctoral researcher at ETH Zurich collaborating with [Prof. Niao He](https://odi.inf.ethz.ch/niaohe) and the [ODI group](https://odi.inf.ethz.ch/). Prior to this, I received doctoral degree from the University of Minnesota under the supervision of [Prof. Georgios B. Giannakis](https://sites.google.com/umn.edu/giannakis/home), and then I gained industry experience, dedicating a year to LLMs.


**Find me** via `bingtsongli[@]gmail.com` or `bingcong.li[@]inf.ethz.ch`.


General interests
-----------

<!-- My research leverages optimization to deepen and expand the impact of deep learning. -->
<!-- My primary focus is to understand the optimization dynamics of neural networks and use these insights to make **pretraining, fine-tuning, and inference of LLMs more efficient**. Unlike black-box approaches, my work incorporates **architectural characteristics**, such as attention and normalization layers, into the optimization process to accelerate convergence. By bridging theoretical foundations with practical algorithm design, I aim to advance the development of scalable, efficient, and reliable LLM systems.  -->

I make computation more efficient and accessible in the era of LLMs. Modern computing exhibits distinct patterns across domains. I use **optimization** as a unifiying framework to enhance computational efficiency at every level of granularity.

- **Architecutres**: We build cmputational efficient pretraining and finetuning pipelines through a co-design of architecture and optimizer, keeping the gains largely explainable.
- **System management**: When training piplelines are fixed, we maximize cluster throughput with better parallelism and optimal resource allocation, ensuring every FLOP counts.
- **Personalization**: We develop memory-efficient optimization so that users with consumer-grade GPUs can harness the power of reasonably large models.


I enjoy cycling 🚴🏻 outside offices. I also do a bit gym training, but ocationally people tell me my triceps pushdown techniques could use some work.


Recent updates
-----------
- **10/2025.** We are hosting the Efficient LLMs Fine-tuning (ELF) Track in [AI+X summit](https://www.plusx.ai/). See you in October, Zurich!
- **07/2025.** I will talk about Riemannian optimization and its provable merits for fine-tuning LLMs in EUROPT 2025.
- **06/2025.** I will talk about "LoRA sugery" at [Efficient Machine Learning Reading Group](https://sites.google.com/view/efficientml).
- **06/2025.** [New paper] LoRA does not use allocated rank effectively. This can be addressed with PoLAR, a co-design of architecture and optimizer. Check out our [paper](https://arxiv.org/abs/2506.03133).
- **06/2025.** [New paper] RefLoRA optimally rescales/refactorizes LoRA per training step to make fine-tuning LLMs faster. Check out our [paper](https://arxiv.org/abs/2505.18877).
- **06/2025.** [New paper] Zeroth-order methods provably find flat minima. Check it out [here](https://arxiv.org/pdf/2506.05454).
- **05/2025.** [ICML 2025] Transfer learning provably benefits RLHF. Check out our [paper](https://arxiv.org/abs/2502.19255v3).
- **04/2025.** Talked about "Fine-tuning LLMs cost-efficiently" at Peking University.
- **01/2025.** [ICLR 2025] We prove that [initialization exponentially impacts the convergence behavior of ScaledGD](https://arxiv.org/abs/2410.18965) on LoRA type problems (i.e., linear --> quadratic rates). 
- **12/2024.** Talked about "Architecture-Aware Optimization" at ELLIS UnConference.
- **12/2024.** [ICASSP 2025] A new variant of SAM is released.
- **09/2024.** [NeurIPS 2024] We study the [implicit regularization of sharpness-aware minimization](https://arxiv.org/abs/2410.14802) (SAM) and explicify it to alleviate computational burdern of SAM. The resultant approach is useful for finetuning LLMs with LoRA.
- **05/2024.** [ICML 2024] [Memory-efficient private finetuning for LLMs](https://arxiv.org/pdf/2310.09639). We also have [a paper](https://openreview.net/pdf?id=chI7jvNkwK) at Theoretical Foundations of Foundation Models (TF2M) workshop. 
- **01/2024.** Start as a postdoc in ETH Zurich, working with Prof. Niao He. 
- **12/2023.** [ICASSP 2024] Universal 'preconditioner' for meta learning.
- **09/2023.** [NeurIPS 2023] Improving generalization by refining optimization of sharpness-aware minimization; see [here](https://arxiv.org/abs/2309.15639).
