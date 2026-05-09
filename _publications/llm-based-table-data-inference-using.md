---
title: "LLM-based Table Data Inference using Data Augmentation and Few-Shot Prompting"
collection: publications
category: domestic
permalink: /publication/table-data-augmentation
excerpt: 'This paper accepted in HCLT-KACL 2024 (poster)'
date: 2024-09-17
venue: 'HCLT-KACL 2024'
slidesurl: ''
paperurl: ''
codeurl: ''
projecturl: ''
citation: 'Lee, J., Hong, M., Lee, E., & Kim, J. (2024). LLM-based Table Data Inference using Data Augmentation and Few-Shot Prompting. In Annual Conference on Human and Language Technology (pp. 587-589). Human and Language Technology.'
image: 'assets/images/publications/llm_based.jpg'
abstract: '표 일부분에 대한 해석은 대규모 언어 모델이 표의 내용을 인식할 수 있는 형태로 구성하여 해석을 생성 하는 태스크다. 기존 연구들은 태스크에 맞는 데이터를 구축하거나 고성능의 LLM 모델을 미세 조정함으 로써, 상황에 맞는 태스크 해결에 초점을 두고 있다. 하지만 파라미터 수가 많아진 LLM 모델을 미세 조정 하기에 많은 자원과 시간이 소요된다. 따라서 한정된 자원으로도 유사한 결과를 낼 수 있도록 기존의 작 은 파라미터를 갖는 모델을 통해 텍스트 생성에 기초적인 틀을 마련하고, LLM 모델의 문장 수정 방식을 통한 2단계 추론 방식을 제안한다. 이 방식을 통해 많은 자원을 이용하여 LLM모델의 미세 조정할 필요없 이, 빠르고 효율적으로 표 일부에 대한 추론을 할 수 있다.'
authors: ''
selected: false
published: true
---

### Overview
This project explores the use of **large language models (LLMs)** for reasoning over tabular data, focusing on how to enhance model performance through **data augmentation** and **few-shot prompting** strategies.  

### Motivation
Despite their strong natural language understanding abilities, LLMs often struggle with structured reasoning tasks involving tables, such as aggregation, comparison, and conditional queries. Traditional table reasoning approaches require specialized architectures or extensive supervised training. This project investigates how far we can push general-purpose LLMs with carefully designed prompting techniques.  

### Approach
- **Data Augmentation:** Synthetic examples are generated to expand the diversity of tabular reasoning cases, covering different table sizes, query types, and logical operations.  
- **Few-Shot Prompting:** Carefully selected exemplars are provided in the prompt to guide the model through reasoning steps on novel tables.  
- **Reasoning Templates:** Chain-of-Thought (CoT) and instruction-style prompts are integrated to elicit structured reasoning from the model.  

### Results
Our experiments show that:
- Data augmentation significantly improves robustness across diverse table types.  
- Few-shot prompting enables LLMs to generalize to new table inference tasks with minimal labeled data.  
- The combined strategy narrows the performance gap between general-purpose LLMs and task-specific table reasoning models.  

### Impact
This study highlights the potential of **prompt engineering and lightweight augmentation** to unlock table reasoning capabilities in LLMs without heavy retraining. The approach provides a scalable way to adapt LLMs for downstream applications in **business analytics, scientific data analysis, and knowledge discovery**.  

---
