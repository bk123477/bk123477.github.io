---
title: "Generating Korean Image Captions using OCR in CoT Prompting"
collection: publications
category: domestic
permalink: /publication/korean-image-captioning
excerpt: 'This paper accepted in HCLT-KACL 2024 (oral)'
date: 2024-09-17
venue: 'HCLT-KACL 2024'
paperurl: ''
codeurl: ''
projecturl: ''
slidesurl: ''
citation: 'Hong, M., Yun, Y., Park, S., & Kim, J. (2024). Generating Korean Image Captions using OCR in CoT Prompting. In Annual Conference on Human and Language Technology (pp. 165-168). Human and Language Technology.'
image: 'assets/images/publications/generating_korean_image_captions_using_ocr.jpg'
abstract: '이미지 캡셔닝은 이미지를 설명하는 문장을 자동으로 생성하는 작업으로, 시각 장애인 지원, 의료 이미지 설명, 비디오 자막 생성 등에서 다양하게 사용된다. 기존 연구들은 다양한 모델을 사용하여 이미지 캡셔닝 작업을 수행해 왔으며 OCR 정보와 같은 추가적인 정보 추출을 통해 이미지를 더 잘 설명하는 캡션을 생 성하고자 하였다. 하지만 영어권 이외의 이미지 캡션 생성 능력은 떨어지는 편이다. 따라서 한국어 이미지 캡션 생성의 성능을 높이고자 OCR 정보를 CoT 프롬프트와 결합하여 최종 캡션을 생성하는 방법을 제안 한다. 이 방법을 통해 기존의 방식에 비교하여 성능 향상을 얻을 수 있으며, 특히 불필요한 정보를 생성하 는 비율을 줄이는 효과가 있다.'
authors: ''
selected: false
published: true
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
