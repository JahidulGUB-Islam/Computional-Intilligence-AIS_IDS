# 🛡️ Intelligent Intrusion Detection System (IDS)

## Advanced Hybrid Intrusion Detection Framework Using Swarm Intelligence, Artificial Immune System, and Ensemble Learning

---

## 📖 Project Overview

This project presents an advanced and explainable **Intelligent Intrusion Detection System (IDS)** designed for modern network and IoT security environments. The proposed framework integrates:

- **Swarm Intelligence**
- **Artificial Immune System (AIS)**
- **Ensemble Machine Learning**
- **Explainable Artificial Intelligence (XAI)**

to improve intrusion detection accuracy, reduce false positives, and enhance detection of minority and zero-day attack patterns.

The framework employs a **Security-Aware and Class-Aware Particle Swarm Optimization (PSO)** algorithm for optimal feature selection and an enhanced **Negative Selection Algorithm (NSA)** for intelligent anomaly detector generation. Furthermore, multiple machine learning and deep learning classifiers including **MLP**, **Random Forest**, and **XGBoost** are combined using ensemble voting strategies to improve detection robustness and generalization capability.

To enhance transparency and interpretability, the system integrates **SHAP-based Explainable AI (XAI)** analysis for feature contribution visualization and model decision interpretation.

The proposed IDS framework is evaluated using widely used benchmark cybersecurity datasets:

- **NSL-KDD** — Classical Intrusion Detection Dataset
- **UNSW-NB15** — Modern Network Attack Dataset
- **CICIoT2023** — Large-Scale IoT Intrusion Dataset

---

# ✨ Core Features

- ✅ Security-Aware and Class-Aware PSO Feature Selection
- ✅ Improved Negative Selection Algorithm (NSA)
- ✅ AIS-Based Hybrid Anomaly Feature Engineering
- ✅ Ensemble Learning Framework (MLP + RF + XGBoost)
- ✅ Hard Voting and Soft Voting Ensemble Strategies
- ✅ 10-Fold Cross-Validation
- ✅ ROC Curve and Precision-Recall Analysis
- ✅ SHAP-Based Explainable AI (XAI)
- ✅ Confusion Matrix Visualization
- ✅ Automatic Result and Figure Saving
- ✅ Reproducible Experimental Setup

---

# 🧠 Proposed Framework Architecture

```text
📂 Dataset Acquisition
          ↓
🧹 Data Cleaning & Preprocessing
          ↓
🔤 Encoding & Feature Standardization
          ↓
🧠 Security-Aware PSO Feature Selection
          ↓
🛡️ Improved AIS-Based Negative Selection
          ↓
⚙️ Hybrid Feature Construction
          ↓
🤖 MLP, RF & XGBoost Training
          ↓
🤝 Ensemble Voting Mechanism
          ↓
📈 Cross-Validation & Performance Evaluation
          ↓
🔍 SHAP Explainability Analysis
          ↓
💾 Result & Model Saving
```

---

# 🖥️ Experimental Environment

| Component | Specification |
|---|---|
| Programming Language | Python 3.x |
| Development Platform | Google Colab |
| Hardware Support | GPU Runtime Recommended |
| Storage | Google Drive |
| Deep Learning Framework | TensorFlow / Keras |

---

# 📦 Required Dependencies

Install all required libraries before running the notebook.

```bash
pip install -q numpy pandas matplotlib seaborn scikit-learn tensorflow xgboost shap
```

---

# 📂 Dataset Configuration

Store the datasets in Google Drive using the following directory structure:

```text
/content/drive/MyDrive/Computational_Intelligence/NSL_KDD
/content/drive/MyDrive/Computational_Intelligence/CICIoT2023
/content/drive/MyDrive/Computational_Intelligence/UNSW_NB15
```

## Example Dataset Structure

```text
NSL_KDD/
├── KDDTrain.csv
└── KDDTest.csv
```

---

# 🚀 Reproduction Procedure

## 🔹 Step 1: Open the Google Colab Notebook

Launch the provided notebook using Google Colab.

---

## 🔹 Step 2: Mount Google Drive

```python
from google.colab import drive
drive.mount('/content/drive')
```

---

## 🔹 Step 3: Configure Dataset Path

```python
dataset_path = '/content/drive/MyDrive/Computational_Intelligence/NSL_KDD'
```

---

## 🔹 Step 4: Data Preprocessing

The preprocessing pipeline includes:

- Missing Value Handling
- Label Cleaning
- Categorical Encoding
- Feature Normalization
- Feature Standardization

---

## 🔹 Step 5: Security-Aware PSO Feature Selection

### ⚙️ PSO Configuration

| Parameter | Value |
|---|---|
| Number of Particles | 20 |
| Maximum Iterations | 25 |
| Inertia Weight | 0.72 |
| Cognitive Coefficient | 1.49 |
| Social Coefficient | 1.49 |

---

## 🔹 Step 6: AIS Detector Generation

### ⚙️ Negative Selection Parameters

| Parameter | Value |
|---|---|
| Number of Detectors | 1000 |
| Mutation Factor | 0.08 |
| Self-Distance Threshold | 0.6 |

---

## 🔹 Step 7: Hybrid Feature Engineering

Generate a hybrid feature space by combining:

- Optimized PSO-selected features
- AIS-generated anomaly-aware features

---

## 🔹 Step 8: Model Training

### 🤖 Implemented Models

- Multi-Layer Perceptron (MLP)
- Random Forest (RF)
- XGBoost
- Hard Voting Ensemble
- Soft Voting Ensemble

---

## 🔹 Step 9: Cross-Validation

Perform **10-Fold Cross-Validation** to ensure generalized and unbiased model evaluation.

---

## 🔹 Step 10: Performance Evaluation

### 📊 Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC
- PR-AUC
- Confusion Matrix
- Attack Detection Rate (ADR)

---

## 🔹 Step 11: Explainability Analysis

SHAP explainability is integrated to:

- Interpret model decisions
- Identify important intrusion features
- Improve model transparency
- Support trustworthy AI-based cybersecurity analysis

---

## 🔹 Step 12: Result Saving

Automatically save:

- Trained Models
- Performance Metrics
- SHAP Visualizations
- ROC Curves
- Confusion Matrices
- Experimental Figures

---

# 🔁 Reproducibility Configuration

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

# 📊 Experimental Results

The proposed framework achieved highly competitive intrusion detection performance across benchmark datasets.

| Performance Metric | Result |
|---|---|
| Accuracy | 99.67% |
| Recall | 99.23% |
| Attack Detection Rate | 99.76% |

---

# 📌 Research Contributions

- Proposed a Security-Aware and Class-Aware PSO-based feature optimization framework
- Developed an enhanced AIS-based Negative Selection Algorithm for anomaly detection
- Designed a hybrid anomaly-aware feature engineering strategy
- Integrated ensemble learning for improved intrusion detection robustness
- Applied SHAP-based explainability for interpretable cybersecurity analytics
- Evaluated the framework on multiple benchmark IDS datasets

---

# 📝 Important Notes

- Use the same random seed to reproduce experimental results
- Update dataset paths according to your Google Drive configuration
- GPU runtime is strongly recommended for efficient deep learning training
- PSO optimization and AIS detector generation may require additional computation time for large-scale datasets

---

# 👨‍💻 Author

**Md. Jahidul Islam**  
Department of Information Technology  
Georgia Southern University

---

# 📄 License

This project is licensed under the **MIT License**.

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

`Intrusion Detection System (IDS)` • `Cybersecurity` • `Artificial Immune System` • `Particle Swarm Optimization` • `XGBoost` • `Random Forest` • `MLP` • `SHAP Explainability` • `IoT Security` • `Ensemble Learning` • `Explainable AI`
