🛡️ Intelligent Intrusion Detection System (IDS)
---
📖 Overview
This project implements an intelligent Intrusion Detection System (IDS) that combines Swarm Intelligence, Artificial Immune System (AIS), and Ensemble Learning for robust attack detection in network and IoT environments. The proposed framework uses a security-aware and class-aware Particle Swarm Optimization (PSO) algorithm for feature selection, an improved Negative Selection Algorithm (NSA) for anomaly detector generation, and multiple classifiers including MLP, Random Forest, and XGBoost.
The framework is evaluated on benchmark IDS datasets including CICIoT2023, NSL-KDD, and UNSW-NB15. The system also integrates SHAP-based explainability for transparent and interpretable intrusion detection.

---

✨ Main Features

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

---
🖥️ Required Environment:

Python 3.x

Google Colab

GPU Runtime Recommended

Google Drive Mounted

---
📦 Required Dependencies
python
numpy
pandas
matplotlib
seaborn
scikit-learn
tensorflow
xgboost
shap

---
Install missing packages:
bash
!pip install -q xgboost shap

---
📂 Dataset Setup
Place datasets in Google Drive:

/content/drive/MyDrive/Computational_Intelligence/NSL_KDD

/content/drive/MyDrive/Computational_Intelligence/CICIoT2023

/content/drive/MyDrive/Computational_Intelligence/UNSW_NB15

Example:

NSL_KDD/
├── KDDTrain.csv
└── KDDTest.csv

---
🚀 Steps to Reproduce Results:

🔹 Step 1: Open the Colab Notebook
Open the provided Colab notebook.

🔹 Step 2: Mount Google Drive:

from google.colab import drive
drive.mount('/content/drive')

🔹 Step 3: Set Dataset Path

dataset_path = '/content/drive/MyDrive/Computational_Intelligence/NSL_KDD'

🔹 Step 4: Run Data Preprocessing
Label Cleaning
Categorical Encoding
Missing Value Handling
Feature Standardization

🔹 Step 5: Run PSO Feature Selection
⚙️ PSO Parameters
Particles: 20
Iterations: 25
Inertia: 0.72
Acceleration coefficients: 1.49, 1.49


🔹 Step 6: Generate AIS Detectors
⚙️ AIS Parameters

Number of detectors: 1000
Mutation factor: 0.08
Self-distance threshold: 0.6

🔹 Step 7: Create Hybrid Features: PSO-selected features + AIS anomaly features

🔹 Step 8: Train Models:
🧠 MLP
🌲 Random Forest
⚡ XGBoost
🤝 Hard Voting Ensemble
🤝 Soft Voting Ensemble

🔹 Step 9: Perform 10-Fold Cross-Validation

🔹 Step 10: Evaluate Performance:
Metrics:
Accuracy
Precision
Recall
F1-score
ROC-AUC
PR-AUC
Confusion Matrix

🔹 Step 11: Run SHAP Explainability: Analyze feature contributions and model transparency.

🔹 Step 12: Save Results: Output directory

---
🔁 Reproducibility

SEED = 42
np.random.seed(SEED)
random.seed(SEED)
tf.random.set_seed(SEED)

---
📊 Expected Results

✅ Attack Detection Rate: 99.76%  
✅ Accuracy: 99.67%  
✅ Recall: 99.23%

---
🔄 Project Workflow

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

---
📝 Notes
Use the same random seed to reproduce results.
Update dataset paths according to your Google Drive structure.
GPU runtime is recommended for faster MLP training.
PSO and AIS detector generation may take time for large datasets.

---

