---
title: 'New preprint on arXiv! 📄'
date: 2026-02-22
permalink: /posts/2026/02/i2i-bias-arxiv/
tags:
  - arXiv
  - Preprint
  - Fairness
---

Excited to share our new preprint, "Evaluating Demographic Misrepresentation in Image-to-Image Portrait Editing," now available on arXiv! 📄

While demographic bias in text-to-image (T2I) generation is well studied, demographic-conditioned failures in instruction-guided image-to-image (I2I) editing remain underexplored. Our work is the first to systematically examine and formalize how identical edit instructions can yield systematically different outcomes across subject demographics in open-weight I2I editors.

## 💡 Key Contributions

1️⃣ **Two Failure Modes**: We define and characterize *Soft Erasure*, where requested edits are silently weakened or ignored, and *Stereotype Replacement*, where edits introduce unrequested, stereotype-consistent attributes (e.g., skin lightening, gender change).

2️⃣ **Controlled Benchmark**: We create a systematic evaluation framework using 84 factorially sampled FairFace portraits spanning race, gender, and age, paired with diagnostic prompts—yielding 5,640 edited images across three open-weight I2I editors.

3️⃣ **Prompt-Level Mitigation**: We demonstrate that a prompt-level identity-preserving control can substantially reduce demographic change for minority groups without model updates, revealing asymmetric identity priors in current editors.

Our findings establish identity preservation as a central and demographically uneven failure mode in I2I editing, motivating the development of demographic-robust editing systems.

You can find our paper at this link: [https://arxiv.org/abs/2602.16149](https://arxiv.org/abs/2602.16149)

Project page: [https://seochan99.github.io/i2i-demographic-bias](https://seochan99.github.io/i2i-demographic-bias)
