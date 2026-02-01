# Tone-Bias-in-Skin-Cancer
Identifying Tone Bias in Skin Cancer using CNN
flowchart LR
    A[ISIC Dermoscopic Images] --> B[Metadata Filtering<br/>Diagnosis + Fitzpatrick Skin Type]
    B --> C[Skin Tone Grouping<br/>Light vs Dark]
    C --> D1[Imbalanced Dataset]
    C --> D2[Balanced Dataset]

    D1 --> E1[Custom CNN]
    D1 --> F1[VGG16 Transfer Learning]

    D2 --> E2[Custom CNN]
    D2 --> F2[VGG16 Transfer Learning]

    E1 --> G[Performance Metrics]
    F1 --> G
    E2 --> G
    F2 --> G

    G --> H[Fairness Analysis<br/>Tone Disparate Impact<br/>Sensitivity by Tone<br/>MCC, ROC-AUC]
