---
title: 'EACL 2026 (Findings) paper accepted! 🎉'
date: 2026-01-04
permalink: /posts/2026/01/visdot-eacl-accepted/
tags:
  - EACL 2026
  - Findings
  - Conference
---

Excited to share that our paper, "VisDoT: Enhancing Visual Reasoning through Human-Like Interpretation Grounding and Decomposition of Thought," has been accepted to **EACL 2026 (Findings)**! 🎉

While recent large vision-language models (LVLMs) show strong language-centric reasoning capabilities, they often struggle with **perceptual grounding**, failing to reliably align visual primitives (e.g., position, length, color, and patterns) with semantic reasoning—especially in visualized data such as charts and graphs.

## 💡 Key Contributions

VisDoT addresses this limitation by combining two key ideas:

1️⃣ **Human-like interpretation grounding** based on graphical perception theory. We formalize four core perceptual tasks—**Position, Length, Pattern, and Extract**—to explicitly guide models toward accurate visual decoding before reasoning.

2️⃣ **Decomposition-of-Thought (DoT) prompting**, which reformulates visual question answering as a compositional process. DoT decomposes complex questions into sequential **perception-oriented and logic-oriented sub-questions**, enabling structured, interpretable, and grounded reasoning within a single model and a single inference pass.

## 🔍 Major Results

Extensive experiments demonstrate that VisDoT substantially improves performance on challenging chart reasoning benchmarks such as **ChartQA**, **ChartQAPro**, and the newly introduced **VisDoTQA**:

*   **Significant Improvement:** Achieve up to **+33.2% absolute improvement** on VisDoTQA.
*   **Strong Performance:** Match or surpass strong closed-source models (e.g., GPT-4o) on ChartQAPro.
*   **Zero-Shot Generalization:** Exhibit **consistent zero-shot gains** on open-domain VQA benchmarks, indicating strong generalization beyond charts.

Overall, VisDoT shows that **explicit perceptual grounding combined with structured thought decomposition** is a powerful and general strategy for reliable and interpretable visual reasoning.
