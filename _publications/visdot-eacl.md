---
title: "VisDoT : Enhancing Visual Reasoning through Human-Like Interpretation Grounding and Decomposition of Thought"
collection: publications
category: conferences
permalink: /publication/visdot
excerpt: 'EACL 2026 (Findings)'
date: 2025-07-28
venue: 'EACL 2026 (Findings)'
# paperurl: 
# citation: 
---
Under-review
=====

Excited to share that our paper, "VisDoT : Enhancing Visual Reasoning through Human-Like Interpretation Grounding and Decomposition of Thought," has been accepted to EACL 2026 (Findings)! 🎉

This work introduces **VisDoT**, a framework for improving visual reasoning in large vision-language models (LVLMs), with a particular focus on **visualized data such as charts and graphs** :contentReference[oaicite:0]{index=0}.  
While recent LVLMs show strong language-centric reasoning capabilities, they often struggle with **perceptual grounding**, failing to reliably align visual primitives (e.g., position, length, color, and patterns) with semantic reasoning.

VisDoT addresses this limitation by combining two key ideas:

1️⃣ **Human-like interpretation grounding** based on graphical perception theory.  
We formalize four core perceptual tasks—**Position, Length, Pattern, and Extract**—to explicitly guide models toward accurate visual decoding before reasoning :contentReference[oaicite:1]{index=1}.

2️⃣ **Decomposition-of-Thought (DoT) prompting**, which reformulates visual question answering as a compositional process.  
DoT decomposes complex questions into sequential **perception-oriented and logic-oriented sub-questions**, enabling structured, interpretable, and grounded reasoning within a single model and a single inference pass :contentReference[oaicite:2]{index=2}.

Extensive experiments demonstrate that VisDoT substantially improves performance on challenging chart reasoning benchmarks such as **ChartQA**, **ChartQAPro**, and the newly introduced **VisDoTQA**.  
Notably, models trained with VisDoT:
- Achieve up to **+33.2% absolute improvement** on VisDoTQA,
- Match or surpass strong closed-source models (e.g., GPT-4o) on ChartQAPro,
- And exhibit **consistent zero-shot gains** on open-domain VQA benchmarks, indicating strong generalization beyond charts :contentReference[oaicite:3]{index=3}.

Overall, VisDoT shows that **explicit perceptual grounding combined with structured thought decomposition** is a powerful and general strategy for reliable and interpretable visual reasoning.
