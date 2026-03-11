# Social Network Ads: Purchase Prediction with KNN

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Latest-orange.svg)
![Accuracy](https://img.shields.io/badge/Accuracy-93%25-green.svg)

## 📌 Project Overview
This project focuses on predicting consumer behavior—specifically whether a user will purchase a product—based on demographic data (Age and Estimated Salary). The core of the project involves implementing the **K-Nearest Neighbors (KNN)** algorithm and evaluating its performance through various metrics and visualizations.

## 🛠️ Data Processing & Methodology
* **Domain-Specific Encoding:** Gender was manually encoded as `Female = 1` and `Male = 0`, prioritizing the higher purchasing frequency observed in the female demographic.
* **Feature Selection:** Through experimentation, it was found that **Age** and **Salary** are the primary drivers of purchase decisions.
* **Preprocessing:** Implemented `StandardScaler` to normalize feature scales, a crucial step for distance-based algorithms like KNN.
* **Model Benchmarking:** Used `LazyPredict` to compare over 30 classifiers, confirming that KNN is among the top-performing models for this dataset.

## 🚀 Model Performance (KNN)
The final model demonstrates high precision and excellent generalization on unseen data.

| Metric | Result |
| :--- | :--- |
| **Model Accuracy** | **93.00%** |
| **Training Accuracy** | **91.00%** |
| **10-Fold Cross-Validation Mean** | **90.67%** |
| **F1-Score (Purchased)** | **0.89** |
| **F1-Score (Not Purchased)** | **0.95** |

### Detailed Classification Report:
```text
               precision    recall  f1-score   support
Not Purchased       0.96      0.94      0.95        68
    Purchased       0.88      0.91      0.89        32

👤 Author
Emre Zorlu

Kaggle: emrezorlu1239
GitHub: emrezorlu1239
