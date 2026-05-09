---
title: "Exposing Blindspots: Cultural Bias Evaluation in Generative Image Models"
collection: publications
category: conferences
permalink: /publication/ecb
excerpt: 'Our paper is now public on the arXiv!'
date: 2025-10-25
venue: 'IASEAI 2026'
# slidesurl: 
paperurl: 'https://arxiv.org/abs/2510.20042'
projecturl: 'https://seochan99.github.io/ECB/'
codeurl: 'https://github.com/cmubig/ECB'
# bibtexurl: 
# citation: 
image: 'assets/images/publications/exposing_blindspot.png'
abstract: 'Generative image models produce striking visuals yet often misrepresent culture. Prior work has examined cultural bias mainly in text-to-image (T2I) systems, leaving image-to-image (I2I) editors underexplored. We bridge this gap with a unified evaluation across six countries, an 8-category/36-subcategory schema, and era-aware prompts, auditing both T2I generation and I2I editing under a standardized protocol that yields comparable diagnostics. Using open models with fixed settings, we derive cross-country, cross-era, and cross-category evaluations. Our framework combines standard automatic metrics, a culture-aware retrieval-augmented VQA, and expert human judgments collected from native reviewers. To enable reproducibility, we release the complete image corpus, prompts, and configurations. Our study reveals three findings: (1) under country-agnostic prompts, models default to Global-North, modern-leaning depictions that flatten cross-country distinctions; (2) iterative I2I editing erodes cultural fidelity even when conventional metrics remain flat or improve; and (3) I2I models apply superficial cues (palette shifts, generic props) rather than era-consistent, context-aware changes, often retaining source identity for Global-South targets. These results highlight that culture-sensitive edits remain unreliable in current systems. By releasing standardized data, prompts, and human evaluation protocols, we provide a reproducible, culture-centered benchmark for diagnosing and tracking cultural bias in generative image models.'
authors: ''
selected: 2
---
Thrilled to share that our paper, "Exposing Blindspots: Cultural Bias Evaluation in Generative Image Models" is now public on the arXiv!

While generative image models produce striking visuals , they frequently misrepresent culture. Prior work primarily focused on text-to-image (T2I) systems, leaving image-to-image (I2I) editors largely unexamined. Our study closes this gap with a unified, reproducible evaluation that audits both T2I generation and I2I editing under a standardized protocol. We offer a culture-centered pipeline for diagnosing and tracking progress in generative image research.

<figure>
  <img src="/images/publications/ecb.png" alt="Representative cultural biases" style="max-width: 800px;">
  <figcaption><strong>Figure 1.</strong> Representative cultural biases in T2I generation across six countries.</figcaption>
</figure>

## 💡 Key Contributions and Experiment Design

Our evaluation framework spans six countries (**China, India, Kenya, Korea, Nigeria, U.S.**), an **8-category/36-subcategory schema**, and uses **era-aware prompts** (traditional, modern, era-agnostic).

### Innovative Experimental Protocols:
We compare inherent T2I bias with I2I editing capability using three complementary studies:

* **Multi-Loop Edit:** Sequential edits testing stability and cultural fidelity under iteration.
* **Attribute Addition:** Stepwise insertion of five distinct culture-specific attributes to quantify cumulative competence (e.g., background, local-script text, food, clothing, accessories).
* **Cross-Country Restylization:** Assessing coherent style transfer from a source country to a target country.

### Multi-Layered Evaluation Framework:
Our platform integrates:

* Standard automatic measures (CLIPScore, DreamSim, Aesthetic Score).
* A **culture-aware metric** that combines retrieval-augmented VQA with curated knowledge.
* Expert **human judgments** collected on a web platform from country-native reviewers (**emic expertise**).

### Data Release for Reproducibility:
We release the complete image corpus from both studies, alongside prompts and configurations, enabling downstream analyses without costly re-running of pipelines.

---

## 🔍 Three Recurring Findings

Our comprehensive study reveals systematic failures in current generative models.

* **Global-North Default:** Under country-agnostic prompts, models default to **Global-North, modern-leaning depictions**. This flattens cross-country distinctions, reducing separability between culturally distinct neighbors (e.g., China $\leftrightarrow$ Korea, Kenya $\leftrightarrow$ Nigeria).
* **Metric-Human Gap in I2I:** Iterative I2I editing erodes cultural fidelity, even when conventional metrics remain flat or improve. By contrast, expert ratings (HQS) and our culture-aware metric both register this degradation.
* **Shortcut Editing:** I2I models tend to apply **superficial cues** (palette shifts, generic props) rather than context- and era-consistent changes. When restylizing to Global-South targets, models frequently retain the source subject's **identity (e.g., race/skin tone)** and often drift toward non-photorealistic styles.

Taken together, these results indicate that culture-sensitive edits remain **unreliable** in current systems. Progress requires moving beyond general-purpose metrics and incorporating **culture- and category-aware evaluation**.

---

You can find our paper at this link: [https://arxiv.org/abs/2510.20042](https://arxiv.org/abs/2510.20042)