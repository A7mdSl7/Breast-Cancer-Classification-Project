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
