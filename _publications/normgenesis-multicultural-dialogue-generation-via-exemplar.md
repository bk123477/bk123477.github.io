---
title: "NormGenesis: Multicultural Dialogue Generation via Exemplar-Guided Social Norm Modeling and Violation Recovery"
collection: publications
category: conferences
permalink: /publication/normgenesis
excerpt: 'Our paper is now public on the arXiv!'
date: 2025-08-19
venue: 'EMNLP 2025'
slidesurl: ''
paperurl: 'https://arxiv.org/abs/2509.18395'
codeurl: 'https://github.com/bk123477/NormGenesis'
projecturl: 'https://bk123477.github.io/NormGenesis/'
# bibtexurl: 
# citation: 
image: '/assets/images/publications/normgenesis.jpg'
abstract: 'Social norms govern culturally appropriate behavior in communication, enabling dialogue systems to produce responses that are not only coherent but also socially acceptable. We present NormGenesis, a multicultural framework for generating and annotating socially grounded dialogues across English, Chinese, and Korean. To model the dynamics of social interaction beyond static norm classification, we propose a novel dialogue type, Violation-to-Resolution (V2R), which models the progression of conversations following norm violations through recognition and socially appropriate repair. To improve pragmatic consistency in underrepresented languages, we implement an exemplar-based iterative refinement early in the dialogue synthesis process. This design introduces alignment with linguistic, emotional, and sociocultural expectations before full dialogue generation begins. Using this framework, we construct a dataset of 10,800 multi-turn dialogues annotated at the turn level for norm adherence, speaker intent, and emotional response. Human and LLM-based evaluations demonstrate that NormGenesis significantly outperforms existing datasets in refinement quality, dialogue naturalness, and generalization performance. We show that models trained on our V2R-augmented data exhibit improved pragmatic competence in ethically sensitive contexts. Our work establishes a new benchmark for culturally adaptive dialogue modeling and provides a scalable methodology for norm-aware generation across linguistically and culturally diverse languages.'
authors: ''
selected: 1
published: true
---
Excited to share that our paper, “NormGenesis: Multicultural Dialogue Generation via Exemplar-Guided Social Norm Modeling and Violation Recovery,” has been accepted to the Main Conference of EMNLP 2025! 🎉
This work addresses a key limitation of large language models (LLMs): their inability to adequately reflect social norms and generate high-quality dialogues in low-resource languages.

<figure>
  <img src="/images/publications/normgenesis.png" alt="NormGenesis pipeline" style="max-width: 800px;">
  <figcaption><strong>Figure 1.</strong> Overview of the <em>NormGenesis</em> pipeline.</figcaption>
</figure>

With NormGenesis, we:
1️⃣ Built culturally appropriate, high-quality dialogue datasets by collecting social norm data from diverse cultures and refining generated dialogues through iterative guidance from a small set of expert exemplars.
2️⃣ Introduced the Violation-to-Resolution (V2R) paradigm, the first systematic framework where conversations not only include norm violations but also the process of realizing and repairing those violations, enabling smoother and more natural dialogues.
3️⃣ Demonstrated that models trained on the NormGenesis dataset significantly outperform those trained on existing social norm or commonsense dialogue datasets, achieving state-of-the-art performance.

You can find our paper at this link: [https://arxiv.org/abs/2509.18395](https://arxiv.org/abs/2509.18395)
