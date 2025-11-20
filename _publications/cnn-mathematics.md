---
title: "Systematic Integration of Attention Modules into CNNs for Accurate and Generalizable Medical Image Diagnosis"
collection: publications
category: manuscripts
permalink: /publication/medical
excerpt: 'Mathematics'
date: 2025-11-19
venue: 'Mathematics'
# slidesurl: 
paperurl: 'https://doi.org/10.3390/math13223728'
# citation: 
---

### Overview
Deep learning has become a critical tool in medical image analysis, yet standard CNNs often struggle to capture subtle and fine-grained features essential for accurate diagnosis. This study systematically integrates attention mechanisms—specifically Squeeze-and-Excitation (SE) and CBAM (Convolutional Block Attention Module)—into five major CNN backbones: VGG16, ResNet18, InceptionV3, DenseNet121, EfficientNetB5.
Across two medical imaging tasks—brain tumor MRI classification and Products of Conception (POC) histopathology classification—the attention-enhanced models consistently outperform their baselines in accuracy, precision, recall, and F1-score.

### Method
1. **Attention Integration Strategy:** The study explores four systematic integration stages:
    - **Baseline:** Use pretrained ImageNet models without modification.
    - **Global SE:** Insert SE blocks after every convolutional block.
    - **Selective SE:** Add SE only to deeper layers (e.g., VGG Blocks 3-5), focusing on semanticaly rich features.
    - **Hybrid Attention (SE + SA):** Combine channel attention (SE) with spatial attention (SA) for enhanced feature localization.
2. **Datasets**
    - **POC dataset:** 4 histopathological tissue classes (chorionic villi, decidual tissue, hemorrhage, trophoblastic tissue).
    - **Brain Tumor MRI dataset (BT-Large-4C):** 4 MRI classes (Normal, Glioma, Meningioma, Pituitary Tumor).
    - Standard preprocessing includes 224×224 resizing and data augmentation (rotation, flipping).

### Experiments
1. **Baseline Performance**
    - **Best baseline:** EfficientNetB5 (POC: 86.05%, BT: 80.50%+)
    - **Weakest baseline:** VGG16
2. **Global SE Integration**: All models improved when SE was applied globally.
    - Example improvement:
        - VGG16 (POC): 78.22% -> **86.65%**
        - EfficientNetB5 (BT) -> 80.50% -> **84.37%**
3. **Selective SE Integration:** Applying SE only to deeper layers achieved even greater gains with less overhead.
    - EfficientNetB5 selective SE achieved:
        - POC: 87.17%
        - Brain Tumor: 86.53%
4. **Hybrid Attention (SE + SA):** Hybrid attention showed the strongest results across both datasets.
    - EfficientNetB5 (SE + SA) achieved:
        - POC Accuracy: **89.97%**, F1: 89.72%
    - ResNet18 (Hybird) strongest on brain tumor dataset:
        - Accuracy: **84.37%**

### Key Findings
- **Hybrid attention (SE + SA) is the most effective strategy,** consistently improving classification accuracy and robustness.
- **Selective integration outperforms global integration,** showing that deeper, semantically meaningful layers benefit the most from attention.
- Even lightweight architectures (e.g., ResNet18, VGG16) benefit significantly when attention is added.
- EfficientNetB5 consistently emerges as the best-performing backbone due to its compound scaling design.

### Contributions
- **A unified comparative framework** applying SE and CBAM across five major CNN architectures.
- Extensive evaluation on **two distinct medical imaging modalities:** pathology (POC) and radiology (MRI).
- Systematic study of where to place attention modules—early, deep, or hybrid.
- Demonstration that **attention enhances both accuracy and interpretability,** especially in nuanced medical image tasks.

### Conclusion
This study demonstrates that attention mechanisms—when integrated thoughtfully—greatly enhance CNN performance for medical image classification. Selective and hybrid attention strategies significantly improve feature localization, channel sensitivity, and overall interpretability. With strong results across two heterogeneous medical datasets, this work provides a robust foundation for future clinical deployment of attention-augmented deep learning models.

You can find our paper at this link: [10.3390/math13223728](10.3390/math13223728)

---