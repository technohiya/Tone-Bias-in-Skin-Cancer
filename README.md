# Tone-Bias-in-Skin-Cancer
Identifying Tone Bias in Skin Cancer using CNN
flowchart LR
    A[Model Predictions] --> B[Split by Skin Tone]
    B --> C1[Light Skin Metrics]
    B --> C2[Dark Skin Metrics]
    C1 --> D[Compare Metrics]
    C2 --> D
    D --> E[Tone Disparate Impact]
    D --> F[Sensitivity Gap]
    D --> G[MCC & ROC-AUC by Group]
