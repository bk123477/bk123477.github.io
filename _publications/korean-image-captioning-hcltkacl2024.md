---
title: "Generating Korean Image Captions using OCR in CoT Prompting"
collection: publications
category: domestic
permalink: /publication/korean-image-captioning
excerpt: 'This paper accepted in HCLT-KACL 2024 (oral)'
date: 2024-09-17
venue: 'HCLT-KACL 2024'
# paperurl: 
citation: 'Hong, M., Yun, Y., Park, S., & Kim, J. (2024). Generating Korean Image Captions using OCR in CoT Prompting. In Annual Conference on Human and Language Technology (pp. 165-168). Human and Language Technology.'
---

### Overview
This project addresses the challenge of generating high-quality image captions in Korean, a language with relatively limited large-scale captioning resources. We integrate **Optical Character Recognition (OCR)** with **Chain-of-Thought (CoT) prompting** to improve captioning performance on text-rich images such as signs, labels, and documents.  

### Motivation
Most vision-language models underperform on Korean due to scarce training data. Text-rich images are especially problematic, as models often ignore or mistranslate embedded Korean text.  

### Approach
- **OCR Integration:** Extract Korean text from images using OCR.  
- **CoT Prompting:** Incorporate OCR outputs into a reasoning chain before generating captions.  
- **Grounded Captions:** Generate captions that combine both visual content and recognized Korean text.  

### Results
Our method produces captions that are more accurate, context-aware, and linguistically faithful to Korean compared to baseline captioning approaches.  

### Impact
This work demonstrates how reasoning-based prompting and OCR integration can improve generative AI for **low-resource languages**, with potential applications in accessibility, digital archiving, and human-centered AI systems.  

---
