---
title: "Proposal of an Improved Fall Detection Using GRU"
collection: publications
category: domestic
permalink: /publication/fall-detection
excerpt: 'This paper accepted in ACK 2023 (undergrad students)'
date: 2023-09-17
venue: 'ACK 2023'
paperurl: ''
codeurl: ''
projecturl: ''
slidesurl: ''
citation: 'Hong, M.-K., Lee, S.-H., & Shin, Y.-S. (2023). Proposal of an Improved Fall Detection Using GRU. Annual Conference of KIPS, 287–288. https://doi.org/10.3745/PKIPS.Y2023M11A.287.'
image: '/assets/images/publications/gru.jpg'
abstract: '우리 사회가 고령화시대로 접어들면서 낙상은 매우 심각한 사회문제가 되고 있으며 정확한 낙 상 감지 기술의 수요도 늘고 있다. 본 연구는 웹 캠을 이용한 개선된 낙상감지 기법을 제안한다. 제 안하는 기법은 RGB 영상을 기반으로 스켈레톤 포즈 추출, 데이터 가공, GRU(Gated Recurrent Unit) 신 경망 알고리즘을 적용한 낙상 감지 실험 및 감지 결과 분석의 과정이 포함된다.'
authors: ''
selected: false
published: true
---

### Overview
As societies age, falls among elderly people are becoming a critical public health issue. Accurate and efficient fall detection technologies are urgently needed. This study proposes an improved **fall detection method using GRU (Gated Recurrent Unit) neural networks**, designed to operate with low-cost devices such as webcams.

### Method
1. **Skeleton Extraction:** Human pose keypoints are extracted from RGB video using PoseNet.  
2. **Feature Engineering:** Three features are computed:
   - **R value:** width-to-height ratio of the human bounding box  
   - **HSSC:** vertical motion speed of head-shoulder segment  
   - **Overlap:** newly introduced metric measuring the overlap between head-shoulder and torso bounding boxes during a fall  
3. **GRU Model:** A stacked GRU network (32 and 64 units with dropout) classifies fall vs. non-fall events.  

### Experiments
- **Datasets:** URFD (UR Fall Detection), AI Hub, and additional self-recorded videos.  
- **Evaluation:** Models with the new *Overlap* feature were compared against baseline GRU models without it.  
- **Performance:** The inclusion of Overlap improved accuracy, precision, and recall:
  - Accuracy: **95.60%** (vs. 94.39%)  
  - Precision: **95.01%** (vs. 94.06%)  
  - Recall: **95.60%** (vs. 93.99%)  
  - AUC-ROC: 0.99  

### Contributions
- Introduced the **Overlap feature**, which captures pose changes during falls and enhances detection accuracy.  
- Demonstrated that the method works with **webcams and low-cost hardware**, without performance delay.  
- Provides a practical basis for integrating fall detection into **real-time applications** such as web or mobile apps.  

### Conclusion
The proposed GRU-based fall detection method significantly improves recognition performance, offering high accuracy and reliability across diverse environments. This approach contributes toward safer monitoring systems for elderly care and can be deployed on resource-constrained devices.  

---
