# Credit-Card-Fraud-Detection
# 💳 Credit Card Fraud Detection System

An end-to-end Machine Learning project to detect fraudulent credit card transactions using highly imbalanced transaction data. The system applies data preprocessing, imbalance handling techniques, multiple ML models, explainability tools, and deployment using FastAPI + Streamlit.

---

## 📌 Project Overview

Credit card fraud is a major challenge in the financial industry. Fraudulent transactions are extremely rare compared to legitimate ones, which makes normal accuracy misleading.

This project builds a fraud detection pipeline that:

* Detects suspicious transactions with high recall
* Minimizes false positives
* Handles extreme class imbalance
* Explains predictions using SHAP
* Provides real-time fraud scoring API
* Includes a Streamlit dashboard

---

## 🚀 Features

✅ Data preprocessing and feature scaling
✅ Handle class imbalance using SMOTE / ADASYN / Class Weights
✅ Train multiple ML models
✅ Threshold optimization for business cost reduction
✅ SHAP explainability
✅ FastAPI real-time prediction API
✅ Streamlit interactive dashboard

---

## 🛠️ Tech Stack

* Python
* Pandas
* NumPy
* Scikit-learn
* XGBoost
* LightGBM
* Imbalanced-learn
* Matplotlib / Seaborn
* SHAP
* FastAPI
* Streamlit

---

## 📂 Project Structure

```bash
credit-card-fraud-detection/
│── data/
│   └── creditcard.csv
│── notebooks/
│   └── fraud_detection.ipynb
│── src/
│   ├── preprocess.py
│   ├── train.py
│   ├── evaluate.py
│── app/
│   ├── main.py
│── models/
│   └── model.pkl
│── requirements.txt
│── README.md
```

---

## 📊 Dataset

Dataset used:

**Kaggle Credit Card Fraud Detection Dataset**

* Total Transactions: 284,807
* Fraud Cases: 492
* Fraud Ratio: 0.17%

Features:

* V1 to V28 (PCA transformed)
* Time
* Amount
* Class

  * 0 = Legitimate
  * 1 = Fraudulent

---

## ⚙️ Workflow

### 1️⃣ Data Preprocessing

* Load dataset
* Handle missing values
* Standardize Time and Amount
* Train/Test split

### 2️⃣ Handle Imbalanced Data

* SMOTE
* ADASYN
* Class Weighting

### 3️⃣ Model Training

Models used:

* Logistic Regression
* Random Forest
* XGBoost
* LightGBM
* Isolation Forest

### 4️⃣ Evaluation Metrics

* Precision
* Recall
* F1 Score
* ROC-AUC
* Precision-Recall AUC
* Confusion Matrix

### 5️⃣ Explainability

* SHAP Summary Plot
* SHAP Waterfall Plot

### 6️⃣ Deployment

* FastAPI REST API
* Streamlit Web App

---

## 📈 Results

Example performance:

| Metric    | Score |
| --------- | ----- |
| Recall    | 0.89  |
| Precision | 0.82  |
| ROC-AUC   | 0.97  |
| F1 Score  | 0.85  |

> Achieved high fraud detection recall while controlling false positives.

---

## ▶️ Installation

```bash
git clone https://github.com/yourusername/credit-card-fraud-detection.git
cd credit-card-fraud-detection
pip install -r requirements.txt
```

---

## ▶️ Run Jupyter Notebook

```bash
jupyter notebook
```

---

## ▶️ Run FastAPI

```bash
uvicorn app.main:app --reload
```

Open:

```bash
http://127.0.0.1:8000/docs
```

---

## ▶️ Run Streamlit

```bash
streamlit run app/dashboard.py
```

---

## 📌 API Example

### POST `/predict`

Input:

```json
{
  "features": [0.1, -1.2, 0.45, ...]
}
```

Output:

```json
{
  "fraud_probability": 0.94,
  "prediction": "Fraud"
}
```

---

## 🔮 Future Enhancements

* Real-time streaming fraud detection
* Kafka event pipeline
* MLflow experiment tracking
* Docker deployment
* Cloud deployment on AWS / GCP
* Federated learning for privacy-preserving training

---

## 💼 Resume Impact

Built a real-time fraud detection system handling extreme class imbalance using SMOTE and XGBoost, achieving high recall and deploying via FastAPI + Streamlit.

---

## 👨‍💻 Author

**Idrisraza Ballary**
AI/ML Engineer Aspirant

* LinkedIn
* GitHub

---

## ⭐ If you like this project

Give it a star on GitHub ⭐
