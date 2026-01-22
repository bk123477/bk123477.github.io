---
title: "Evaluating Demographic Misrepresentation in Image-to-Image Portrait Editing"
collection: publications
category: conferences
permalink: /publication/i2i-bias
excerpt: 'This paper is currently under review.'
date: 2026-01-22
venue: 'Under Review'
# slidesurl: 
# paperurl: 
# bibtexurl: 
# citation: 
---
We are excited to share our latest research on demographic-conditioned failures in instruction-guided image-to-image (I2I) portrait editing. While demographic bias in text-to-image (T2I) generation is well studied, our work is the first to systematically examine and formalize how identical edit instructions can yield systematically different outcomes across subject demographics in open-weight I2I editors.

<figure>
  <img src="/images/publications/i2i-bias.png" alt="I2I Bias Evaluation Framework" style="max-width: 800px;">
  <figcaption><strong>Figure 1.</strong> Overview of demographic-conditioned failures in I2I portrait editing.</figcaption>
</figure>

In this work, we:
1️⃣ **Identify Two Failure Modes**: We define and characterize *Soft Erasure*, where requested edits are silently weakened or ignored, and *Stereotype Replacement*, where edits introduce unrequested, stereotype-consistent attributes (e.g., skin lightening, gender change).

2️⃣ **Introduce a Controlled Benchmark**: We create a systematic evaluation framework using 84 factorially sampled FairFace portraits spanning race, gender, and age, paired with diagnostic prompts—yielding 5,640 edited images across three open-weight I2I editors.

3️⃣ **Propose Prompt-Level Mitigation**: We demonstrate that a prompt-level identity-preserving control can substantially reduce demographic change for minority groups without model updates, revealing asymmetric identity priors in current editors.

Our findings establish identity preservation as a central and demographically uneven failure mode in I2I editing, motivating the development of demographic-robust editing systems.
