---
title: "LLM-based Table Data Inference using Data Augmentation and Few-Shot Prompting"
collection: publications
category: domestic
permalink: /publication/table-data-augmentation
excerpt: 'This paper accepted in HCLT-KACL 2024 (poster)'
date: 2024-09-17
venue: 'HCLT-KACL 2024'
slidesurl: 
paperurl: 
citation: 'Lee, J., Hong, M., Lee, E., & Kim, J. (2024). LLM-based Table Data Inference using Data Augmentation and Few-Shot Prompting. In Annual Conference on Human and Language Technology (pp. 587-589). Human and Language Technology.'
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