````markdown
# 🛡️ Intelligent Intrusion Detection System (IDS)

A robust and explainable Intrusion Detection System (IDS) framework that integrates **Swarm Intelligence**, **Artificial Immune System (AIS)**, and **Ensemble Learning** for advanced cyberattack detection in modern network and IoT environments.

The proposed framework combines:

- Security-aware and class-aware **Particle Swarm Optimization (PSO)** for intelligent feature selection
- Improved **Negative Selection Algorithm (NSA)** for anomaly detector generation
- Hybrid ensemble learning using **MLP**, **Random Forest**, and **XGBoost**
- **SHAP Explainability** for transparent and interpretable cybersecurity analytics

The framework is evaluated on benchmark intrusion detection datasets including:

- NSL-KDD
- UNSW-NB15
- CICIoT2023

---

# 📖 Overview

Modern cyberattacks are increasingly sophisticated, dynamic, and difficult to detect using traditional signature-based intrusion detection systems. This project introduces a hybrid intelligent IDS framework capable of:

- Detecting both known and unknown attacks
- Improving minority attack detection
- Reducing false positives
- Enhancing feature optimization
- Providing explainable AI-driven security insights

The framework leverages biologically inspired and swarm-based optimization techniques together with machine learning and deep learning models to improve overall intrusion detection performance.

---

# ✨ Main Features

✅ Security-aware and class-aware PSO feature selection  
✅ Improved Negative Selection Algorithm (NSA)  
✅ Hybrid AIS-based anomaly feature generation  
✅ Ensemble Learning (MLP + RF + XGBoost)  
✅ Hard Voting and Soft Voting Ensembles  
✅ 10-Fold Cross-Validation  
✅ ROC and Precision-Recall Analysis  
✅ SHAP Explainability  
✅ Confusion Matrix Visualization  
✅ Automatic Result Saving  
✅ Reproducible Experimental Setup  

---

# 🖥️ Required Environment

| Component | Requirement |
|---|---|
| Programming Language | Python 3.x |
| Development Environment | Google Colab |
| Hardware | GPU Runtime Recommended |
| Storage | Google Drive Mounted |

---

# 📦 Required Dependencies

```python
numpy
pandas
matplotlib
seaborn
scikit-learn
tensorflow
xgboost
shap
```

## Install Missing Packages

```bash
pip install -q xgboost shap
```

---

# 📂 Dataset Setup

Place datasets in Google Drive using the following structure:

```text
/content/drive/MyDrive/Computational_Intelligence/NSL_KDD
/content/drive/MyDrive/Computational_Intelligence/CICIoT2023
/content/drive/MyDrive/Computational_Intelligence/UNSW_NB15
```

## Example Structure

```text
NSL_KDD/
├── KDDTrain.csv
└── KDDTest.csv
```

---

# 🚀 Steps to Reproduce Results

## 🔹 Step 1: Open the Colab Notebook

Open the provided Google Colab notebook.

---

## 🔹 Step 2: Mount Google Drive

```python
from google.colab import drive
drive.mount('/content/drive')
```

---

## 🔹 Step 3: Set Dataset Path

```python
dataset_path = '/content/drive/MyDrive/Computational_Intelligence/NSL_KDD'
```

---

## 🔹 Step 4: Run Data Preprocessing

The preprocessing stage includes:

- Label Cleaning
- Missing Value Handling
- Categorical Encoding
- Feature Standardization

---

## 🔹 Step 5: Run PSO Feature Selection

### ⚙️ PSO Parameters

| Parameter | Value |
|---|---|
| Number of Particles | 20 |
| Maximum Iterations | 25 |
| Inertia Weight | 0.72 |
| Acceleration Coefficients | 1.49, 1.49 |

---

## 🔹 Step 6: Generate AIS Detectors

### ⚙️ AIS Parameters

| Parameter | Value |
|---|---|
| Number of Detectors | 1000 |
| Mutation Factor | 0.08 |
| Self-distance Threshold | 0.6 |

---

## 🔹 Step 7: Create Hybrid Features

Combine:

- PSO-selected optimized features
- AIS-generated anomaly features

---

## 🔹 Step 8: Train Models

### 🧠 Machine Learning Models

- Multi-Layer Perceptron (MLP)
- Random Forest (RF)
- XGBoost
- Hard Voting Ensemble
- Soft Voting Ensemble

---

## 🔹 Step 9: Perform 10-Fold Cross-Validation

Cross-validation is used to ensure robust and generalized performance evaluation.

---

## 🔹 Step 10: Evaluate Performance

### 📊 Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- PR-AUC
- Confusion Matrix

---

## 🔹 Step 11: Run SHAP Explainability

SHAP analysis is used to:

- Interpret model decisions
- Identify important security features
- Improve transparency and trustworthiness

---

## 🔹 Step 12: Save Results

All outputs including:

- Metrics
- Figures
- Confusion Matrices
- SHAP Visualizations

are automatically saved to the output directory.

---

# 🔁 Reproducibility

```python
SEED = 42

import numpy as np
import random
import tensorflow as tf

np.random.seed(SEED)
random.seed(SEED)
tf.random.set_seed(SEED)
```

---

# 📊 Expected Results

| Metric | Performance |
|---|---|
| Accuracy | 99.67% |
| Recall | 99.23% |
| Attack Detection Rate | 99.76% |

---

# 🔄 Project Workflow

```text
📂 Dataset Loading
        ↓
🧹 Data Cleaning & Preprocessing
        ↓
🔤 Categorical Encoding & Standardization
        ↓
🧠 Security-Aware PSO Feature Selection
        ↓
🛡️ Improved Negative Selection Algorithm
        ↓
⚙️ Hybrid Feature Construction
        ↓
🤖 MLP, RF & XGBoost Training
        ↓
🤝 Hard & Soft Voting Ensemble
        ↓
📈 Evaluation & Cross-Validation
        ↓
🔍 SHAP Explainability
        ↓
💾 Result Saving
```

---

# 📌 Research Contributions

- Developed a security-aware and class-aware PSO-based feature selection framework
- Proposed an improved AIS-based Negative Selection Algorithm
- Integrated hybrid anomaly-aware feature engineering
- Combined deep learning and ensemble learning for robust IDS performance
- Applied SHAP explainability for transparent cybersecurity analytics
- Evaluated the framework on multiple benchmark IDS datasets

---

# 📝 Notes

- Use the same random seed to reproduce results
- Update dataset paths according to your Google Drive structure
- GPU runtime is recommended for faster MLP training
- PSO and AIS detector generation may take time for large datasets

---

# 👨‍💻 Author

**Md. Jahidul Islam**  
Department of Information Technology  
Georgia Southern University

---

# 📄 License

MIT License

```text
MIT License

Copyright (c) 2026 Md. Jahidul Islam

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software.
```

---

# ⭐ Citation

```bibtex
@article{jahidul2026ids,
  title={Intelligent Intrusion Detection System using Swarm Intelligence, Artificial Immune System, and Ensemble Learning},
  author={Islam, Md. Jahidul},
  journal={Research Project},
  year={2026}
}
```

---

# 🔒 Keywords

`Intrusion Detection System` • `Cybersecurity` • `Artificial Immune System` • `Particle Swarm Optimization` • `XGBoost` • `Random Forest` • `MLP` • `SHAP Explainability` • `IoT Security` • `Ensemble Learning`
````
