---
title: "Toward Trustworthy Portrait Editing: Evaluation of Demographic Misrepresentation in I2I Models"
collection: publications
category: conferences
permalink: /publication/i2i-bias
excerpt: 'Our paper is now public on arXiv!'
date: 2026-02-22
venue: 'Under Review'
slidesurl: ''
paperurl: 'https://arxiv.org/abs/2602.16149'
codeurl: ''
projecturl: 'https://seochan99.github.io/i2i-demographic-bias/'
# bibtexurl: 
# citation: 
image: '/assets/images/publications/evaluating_demographic.png'
abstract: 'Instruction-guided image-to-image (I2I) editors are increasingly entering consumer and professional visual workflows, where trustworthiness depends not only on prompt compliance but also on equitable preservation of identity-relevant attributes. We formalize two failure modes Soft Erasure, where requested edits are weakly realized or silently suppressed, and Stereotype Replacement, where edits introduce unrequested, stereotype-consistent demographic attributes and evaluate them across three recent open-weight editors on 5,040 edited portraits. We find that 62-71% of outputs exhibit skin lightening, with Indian and Black source portraits affected at 72-75% compared with 44\% for White source portraits, a pattern consistent with output-level drift toward lighter or more White-presenting appearances when identity constraints are underspecified. In a mitigation case study, prompt-level appearance constraints reduce race-change scores for non-White source portraits by up to 1.48 points, with negligible change for White source portraits, without modifying model weights. Together, these findings show that identity preservation is not a uniform property of I2I portrait editing systems, but an unevenly distributed trustworthiness failure with direct social consequences. At deployment scale, such silent distortions can shape AI-mediated self-representation and reinforce representational disparities. We introduce a controlled audit protocol for fairness-aware evaluation and governance of generative editing systems.'
authors: ''
selected: false
published: true
---
We are excited to share our latest research on demographic-conditioned failures in instruction-guided image-to-image (I2I) portrait editing. While demographic bias in text-to-image (T2I) generation is well studied, our work is the first to systematically examine and formalize how identical edit instructions can yield systematically different outcomes across subject demographics in open-weight I2I editors.

<figure>
  <img src="/assets/images/publications/i2i_bias.jpg" alt="I2I Bias Evaluation Framework" style="max-width: 800px;">
  <figcaption><strong>Figure 1.</strong> Comparison of I2I portrait editing across diverse demographics. Given identity-agnostic prompts (e.g., "senior executive," "senior military strategist"), baseline methods often produce <em>stereotype replacements</em>—changing race or gender toward majority demographics (red boxes). Our prompt-level mitigation preserves the original identity across all demographic groups (green boxes), demonstrating that identity preservation failures disproportionately affect minority subjects.</figcaption>
</figure>

In this work, we:
1️⃣ **Identify Two Failure Modes**: We define and characterize *Soft Erasure*, where requested edits are silently weakened or ignored, and *Stereotype Replacement*, where edits introduce unrequested, stereotype-consistent attributes (e.g., skin lightening, gender change).

2️⃣ **Introduce a Controlled Benchmark**: We create a systematic evaluation framework using 84 factorially sampled FairFace portraits spanning race, gender, and age, paired with diagnostic prompts—yielding 5,640 edited images across three open-weight I2I editors.

3️⃣ **Propose Prompt-Level Mitigation**: We demonstrate that a prompt-level identity-preserving control can substantially reduce demographic change for minority groups without model updates, revealing asymmetric identity priors in current editors.

Our findings establish identity preservation as a central and demographically uneven failure mode in I2I editing, motivating the development of demographic-robust editing systems.
