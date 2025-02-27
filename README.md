# Diabetes Prediction: Comparing Logistic Regression and Naïve Bayes

This project explores the predictive performance of **Logistic Regression** and **Naïve Bayes** using Kaggle’s **Diabetes Health Indicators** dataset. Implemented in **MATLAB**, the study evaluates these models based on **AUC, F1-score, recall, accuracy, and training/testing time**.  

## 🔹 Project Overview

This project was part of the **Master’s in Data Science** program (Machine Learning course) at **City, University of London** (2024) and was awarded a **Distinction**.

### 🚀 Key Skills Demonstrated  

- **Machine Learning**: Built and compared **Logistic Regression** & **Naïve Bayes** models.  
- **Model Evaluation**: Assessed **AUC, F1-score, accuracy, recall, and precision**.  
- **Feature Selection & Impact Analysis**: Used statistical tests to refine input features.  
- **Programming**: Developed in **MATLAB**, including data preprocessing, training, and evaluation.  

## 📂 Dataset  

- **Source**: Kaggle’s **[Diabetes Health Indicators Dataset](https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset/data)** (BRFSS2015, CDC). *(Not included in this repository.)*  
- **Size**: 253,680 rows, 22 columns (1 binary target, 21 features).  
- **Data Types**: 14 binary, 3 numerical, 4 ordinal; no missing values.  
- **Class Imbalance**: 86% non-diabetes, 14% diabetes.  

## 🏗️ Model Development  

### 📌 Hypothesis  
- **Logistic Regression** is expected to outperform **Naïve Bayes** in **AUC** but not in **accuracy**.  
- **Precision** may be low due to class imbalance.  
- **Naïve Bayes** should train and test faster.  

### ⚙️ Model Selection  
- **Logistic Regression**: Lasso regularization, 10-fold cross-validation, mean coefficients as the final model.  
- **Naïve Bayes**: Chi-squared test & ANOVA for feature selection, full dataset for probability estimation.  

### 🎯 Training & Evaluation  
- **70/30 train-test split**, **10-fold cross-validation** for optimization.  
- Best models tested on **F1-score, accuracy, precision, recall, and AUC**.  

## 📊 Evaluation & Findings  

- **Logistic Regression** outperforms **Naïve Bayes** in **AUC, F1-score, and recall**, aligning with [Zidian Xie et al. (2019)](https://www.cdc.gov/pcd/issues/2019/19_0109.htm).  
- **Naïve Bayes** achieves **higher accuracy and precision**, likely due to the chosen cutoff (0.14 vs. 0.5).  
- **Feature selection significantly influences model effectiveness**; chi-squared & ANOVA have limitations in **Naïve Bayes**.  
- **Naïve Bayes** has a **faster training time**, but **Logistic Regression** achieves **faster testing**.  
- **Class imbalance** impacts model performance, particularly accuracy.  

## ⚡ Conclusion  

**Logistic Regression** excels in **AUC and F1-score**, while **Naïve Bayes** is **faster and more accurate** in terms of precision. **Feature selection** and **class imbalance** significantly affect model outcomes.  

## 📜 License

This project’s code is licensed under the [MIT License](LICENSE).
