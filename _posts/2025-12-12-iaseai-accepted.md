---
title: 'IASEAI 2026 paper accepted! 🎉'
date: 2025-12-12
permalink: /posts/2025/12/iaseai/
tags:
  - IASEAI 2026
  - Conference
---

Excited to share that our paper, "Exposing Blindspots: Cultural Bias Evaluation in Generative Image Models," has been accepted to IASEAI 2026! 🎉

While generative image models produce striking visuals, they frequently misrepresent culture. Prior work primarily focused on text-to-image (T2I) systems, leaving image-to-image (I2I) editors largely unexamined. Our study closes this gap with a unified, reproducible evaluation that audits both T2I generation and I2I editing under a standardized protocol.

## 💡 Key Contributions

Our evaluation framework spans six countries (**China, India, Kenya, Korea, Nigeria, U.S.**), an **8-category/36-subcategory schema**, and uses **era-aware prompts** (traditional, modern, era-agnostic).

We compare inherent T2I bias with I2I editing capability using three complementary studies:
- **Multi-Loop Edit:** Sequential edits testing stability and cultural fidelity under iteration
- **Attribute Addition:** Stepwise insertion of five distinct culture-specific attributes to quantify cumulative competence
- **Cross-Country Restylization:** Assessing coherent style transfer from a source country to a target country

Our platform integrates standard automatic measures (CLIPScore, DreamSim, Aesthetic Score), a **culture-aware metric** that combines retrieval-augmented VQA with curated knowledge, and expert **human judgments** from country-native reviewers.

## 🔍 Three Recurring Findings

1️⃣ **Global-North Default:** Under country-agnostic prompts, models default to Global-North, modern-leaning depictions, reducing separability between culturally distinct neighbors.

2️⃣ **Metric-Human Gap in I2I:** Iterative I2I editing erodes cultural fidelity, even when conventional metrics remain flat or improve.

3️⃣ **Shortcut Editing:** I2I models tend to apply superficial cues rather than context- and era-consistent changes.

You can find our paper at this link: [https://arxiv.org/abs/2510.20042](https://arxiv.org/abs/2510.20042)