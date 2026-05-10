---
title: "PEEM: Prompt Engineering Evaluation Metrics for Interpretable Joint Evaluation of Prompts and Responses in LLMs"
collection: publications
category: manuscripts
permalink: /publication/peem
excerpt: 'Our paper has been published in IEEE Access!'
date: 2026-04-24
venue: 'IEEE Access'
slidesurl: ''
paperurl: 'https://ieeexplore.ieee.org/document/11460151'
codeurl: ''
projecturl: ''
# citation: 
image: '/assets/images/publications/peem.png'
abstract: >-
  Prompt design is a primary control interface for large language models (LLMs), yet standard evaluations largely reduce performance to answer correctness, obscuring why a prompt succeeds or fails and providing little actionable guidance. We propose PEEM (Prompt Engineering Evaluation Metrics), a unified framework for joint and interpretable evaluation of both prompts and responses. PEEM defines a structured rubric with 9 axes: 3 prompt criteria (clarity/structure, linguistic quality, fairness) and 6 response criteria (accuracy, coherence, relevance, objectivity, clarity, conciseness), and uses an LLM-based evaluator to output (i) scalar scores on a 1-5 Likert scale and (ii) criterion-specific natural-language rationales grounded in the rubric. Across 7 benchmarks and 5 task models, PEEM's accuracy axis strongly aligns with conventional accuracy while preserving model rankings (aggregate Spearman rho about 0.97, Pearson r about 0.94, p < 0.001). A multi-evaluator study with four models shows consistent relative judgments (pairwise rho = 0.68-0.85), supporting evaluator-agnostic deployment. Beyond alignment, PEEM captures complementary linguistic failure modes and remains informative under prompt perturbations: prompt-quality trends track downstream accuracy under iterative rewrites, semantic adversarial manipulations induce clear score degradation, and meaning-preserving paraphrases yield high stability (robustness rate about 76.7-80.6%). Finally, using only PEEM scores and rationales as feedback, a zero-shot prompt rewriting loop improves downstream accuracy by up to 11.7 points, outperforming supervised and RL-based prompt-optimization baselines. Overall, PEEM provides a reproducible, criterion-driven protocol that links prompt formulation to response behavior and enables systematic diagnosis and optimization of LLM interactions.
authors: ''
selected: 4
published: true
---

Excited to share that our paper, "**PEEM: Prompt Engineering Evaluation Metrics for Interpretable Joint Evaluation of Prompts and Responses**," has been published in **IEEE Access**! 🎉

This work introduces **PEEM**, a novel framework for the joint evaluation of prompts and model responses. Traditional metrics often focus solely on the output quality, neglecting the critical role of prompt engineering. PEEM addresses this gap by providing interpretable metrics that assess how well a prompt guides the model and how consistently the model responds.

Key highlights:
- **Joint Evaluation**: Simultaneously evaluates prompt quality and response accuracy.
- **Interpretability**: Provides granular insights into prompt-response dynamics.
- **Robustness**: Tested across various LLMs and prompt engineering techniques.

You can find the paper at:
- **IEEE Xplore**: [https://ieeexplore.ieee.org/document/11460151](https://ieeexplore.ieee.org/document/11460151)
- **arXiv**: [https://arxiv.org/abs/2603.10477](https://arxiv.org/abs/2603.10477)
