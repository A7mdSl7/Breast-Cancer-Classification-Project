# Breast Cancer Classification Project

## 📌 Overview
This project implements a binary classification model to predict whether breast cancer tumors are **malignant (M)** or **benign (B)** using the **Wisconsin Breast Cancer Diagnostic Dataset**.  
The model is built using **Logistic Regression in Python**, with steps including:
- Data investigation  
- Visualization  
- Preprocessing  
- Training  
- Evaluation  
- Interpretation  

The goal is to achieve high accuracy while **minimizing false negatives**, which are critical in medical diagnostics.

---

## 📂 Table of Contents
- [Dataset](#dataset)  
- [Installation](#installation)  
- [Usage](#usage)  
- [Project Steps](#project-steps)  
- [Model Details](#model-details)  
- [Results](#results)  
- [Model Interpretation](#model-interpretation)  
- [Contributing](#contributing)  
- [License](#license)  

---

## 📊 Dataset
The project uses the **Breast Cancer Wisconsin (Diagnostic) Dataset** from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/wdbc.data).  

- **Records:** 569  
- **Features:** 30 numerical features (e.g., `radius_mean`, `texture_mean`, `perimeter_mean`, etc.) describing cell nuclei characteristics  
- **Target:** Diagnosis (`M = Malignant`, `B = Benign`)  
- Data is loaded directly from the UCI URL in the notebook.  

---

## ⚙️ Installation
Clone the repository:
```bash
git clone https://github.com/your-username/breast-cancer-classification.git

---

📑 Project Steps

Data Investigation: Load dataset, check for nulls/duplicates, summary statistics.

Data Visualization: Histograms, boxplots, pairplots; check class balance (M vs B).

Data Preprocessing: Encode Diagnosis (M=1, B=0), scale features using StandardScaler, drop ID column.

Train-Test Split: 80/20 split with stratification; handle imbalance using class_weight="balanced".

Model Training: Train Logistic Regression model.

Model Evaluation: Confusion Matrix (heatmap), ROC Curve & AUC, Classification Report (Precision, Recall, F1-score, Accuracy).

Model Interpretation: Analyze coefficients, intercept, and error types (focus on false negatives).

🤖 Model Details

Algorithm: Logistic Regression (class_weight="balanced")

Features: All 30 numerical features after scaling

Preprocessing: Label encoding for target, StandardScaler for features

Evaluation Metrics

Confusion Matrix

ROC AUC

Precision, Recall, F1-Score, Accuracy

📈 Results

The model achieves balanced performance on training and testing sets.

Key metrics:

Accuracy: ~0.96

AUC: ~0.99

Confusion Matrix: Visualized as heatmap

ROC Curve: Plotted with AUC

Class Distribution: ~212 Malignant, ~357 Benign

🔍 Model Interpretation

Coefficients: Positive values ↑ probability of Malignant, negative ↓ it.

Intercept: Baseline log-odds.

Performance: No signs of overfitting/underfitting (similar train/test scores).

Errors: Focus on minimizing false negatives (missed malignant cases).

Medical Implications: Prioritize recall for Malignant class to ensure patient safety.

🤝 Contributing

Contributions are welcome!
Feel free to fork this repository and submit a pull request with improvements, such as:

Alternative models (e.g., Random Forest)

Advanced imbalance handling (e.g., SMOTE)

📜 License

This project is licensed under the MIT License.
See the LICENSE
 file for details.
