# 🩺 Breast Cancer Prediction using Logistic Regression

This project uses **Logistic Regression** to predict whether a breast tumor is **benign (0)** or **malignant (1)** based on features from the **Breast Cancer Wisconsin Diagnostic Dataset**.

---

## 📊 Dataset Overview

The dataset contains features computed from digitized images of fine needle aspirate (FNA) of breast masses. Each record has:

- 30 numerical features (e.g., `radius_mean`, `texture_mean`, `area_mean`, etc.)
- 1 target variable: `diagnosis` (B = Benign, M = Malignant)

---

## 🧪 Workflow

### 🔹 1. Data Cleaning
- Removed irrelevant columns (`Unnamed: 32`, `id`)
- Handled missing values
- Converted diagnosis labels: `M → 1`, `B → 0`

### 🔹 2. Feature Scaling
- Applied `StandardScaler` to normalize all features

### 🔹 3. Train/Test Split
- Split data into 70% training and 30% testing using `train_test_split`

### 🔹 4. Model Training
- Trained a **Logistic Regression** model using Scikit-Learn

### 🔹 5. Evaluation
- Calculated **Accuracy**, **Precision**, **Recall**, **F1-score**
- Displayed **Confusion Matrix**

---

## 🧠 How Logistic Regression Works

Logistic regression models the probability that a tumor is malignant using the **sigmoid function**:

\[
P(y = 1 | x) = \frac{1}{1 + e^{-(w_1x_1 + w_2x_2 + \dots + w_nx_n + b)}}
\]

- If \( P > 0.5 \): Predicts **malignant (1)**
- If \( P ≤ 0.5 \): Predicts **benign (0)**

---

## ✅ Example Results

- **Accuracy:** ~95–97%

---

## 📁 Files in this Project

- `breast_cancer_model.ipynb` – Full notebook with code, output, and explanations
- `data.csv` – Input dataset (should be added manually or via upload)
- `README.md` – Project documentation (you’re reading it!)

---

## 🔧 Requirements

- Python 3.x
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn

Install using:
```bash
pip install pandas numpy scikit-learn matplotlib seaborn

