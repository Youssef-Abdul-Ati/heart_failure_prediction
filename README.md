# 🫀 Heart Failure Prediction using Machine Learning

A production-ready machine learning model to predict heart disease risk from clinical patient data. Built with a focus on **high recall (92.2%)** to minimize missed diagnoses — critical in healthcare applications.

## 📌 Project Overview
This project develops a classification model to predict the presence of heart disease using 12 clinical features such as age, cholesterol, chest pain type, and ECG results. The model is designed not just for accuracy, but for **clinical safety**, prioritizing the detection of true positive cases.

The final pipeline includes:
- Data cleaning and KNN-based imputation
- Feature preprocessing with scikit-learn Pipeline
- Hyperparameter tuning
- Model evaluation with focus on **Recall**
- Risk prediction for new patients
- Deployment-ready saved model

Dataset: [Heart Failure Prediction on Kaggle](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction)

---

## 🎯 Why This Project Stands Out

- ✅ **High Recall (92.2%)**: Minimizes false negatives — patients with heart disease are correctly identified.
- ✅ **Interpretable Model**: Uses **Logistic Regression** instead of black-box models for transparency.
- ✅ **Realistic Predictions**: Well-calibrated probabilities you can trust.
- ✅ **Ready for Deployment**: Model and preprocessor saved as `.pkl` files.
- ✅ **Clinically Relevant**: Designed with medical decision-making in mind.

---

## 📊 Model Performance (Test Set)

| Model               | Accuracy | Recall | ROC AUC |
|---------------------|----------|--------|--------|
| **Logistic Regression** | **0.897** | **0.922** | 0.933 |
| SVM (RBF)           | 0.875    | 0.892  | 0.940 |
| Random Forest       | 0.859    | 0.873  | 0.927 |
| Decision Tree       | 0.739    | 0.765  | 0.736 |

➡️ **Logistic Regression was selected as the final model** due to its superior recall, ensuring 92% of actual heart disease cases are detected.

---

## 🧪 Example Predictions

| Patient | Risk Probability | Prediction |
|--------|------------------|------------|
| Low-risk (40 y/o, no symptoms) | 12.3% | No Heart Disease |
| High-risk (70 y/o, ASY pain, low MaxHR) | 98.7% | Heart Disease |

---

## 📦 Files Included

- `heart_failure.ipynb` – Full Jupyter notebook with EDA, modeling, and evaluation
- `best_model.pkl` – Trained Logistic Regression model
- `preprocessor.pkl` – Fitted preprocessing pipeline
- `app.py` – Streamlit web app (optional)
- `requirements.txt` – Required packages

---

## 🚀 How to Run

1. Clone the repository
   ```bash
   git clone https://github.com/your-username/heart-failure-prediction.git
