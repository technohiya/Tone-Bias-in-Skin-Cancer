# Tone-Bias-in-Skin-Cancer
Identifying Tone Bias in Skin Cancer using CNN
## Overview
This project investigates whether convolutional neural networks (CNNs) used for skin cancer detection exhibit performance bias across different skin tones. Using dermoscopic images and fairness-aware evaluation, the study compares how models behave on lighter vs darker skin tone groups and examines how dataset imbalance contributes to bias.

This project explores:
1. Do CNN-based skin cancer classifiers show tone-based bias?
2. How does dataset imbalance affect fairness?
3. Can balancing the dataset reduce disparities?
4. Do different CNN architectures behave differently in terms of fairness?

## Dataset

Images were sourced from the ISIC Archive, using only samples with:
>Diagnostic labels (benign vs malignant)
>Fitzpatrick Skin Type (FST) annotations

Two datasets were created:
1. Imbalanced dataset – Reflecting real-world distribution (more light skin & benign cases)

2. Balanced dataset – Equalized across skin tones and diagnosis classes to study fairness impact
