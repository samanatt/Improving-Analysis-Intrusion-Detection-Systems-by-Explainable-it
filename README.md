# Explainable Intrusion Detection System (IDS) for IoT Networks

This repository presents an **Explainable Intrusion Detection System (IDS)** for IoT networks, leveraging machine learning and explainability techniques. The system is evaluated on public datasets, including **NF-BoT-IoT-v2** and **NF-ToN-IoT-v2**, to enhance both detection performance and interpretability.

## Features

### 1. **Machine Learning Models**
Six machine learning models were developed and evaluated:
- **LightGBM**
- **Logistic Regression**
- **Decision Tree (DT)**
- **XGBoost**
- **Naive Bayes**
- **Support Vector Machine (SVM)**

The **XGBoost** and **LightGBM** models achieved the highest accuracy and weighted recall across datasets.

### 2. **Feature Selection and Dimensionality Reduction**
- Feature importance was computed using **SHAP (Shapley Additive Explanations)**.
- Dimensionality was reduced from 41 to 10 features, significantly improving training and inference times without compromising detection performance.

### 3. **Explainability**
- **Global Explainability:** SHAP summary plots were used to identify the top contributing features for each class, providing insights into the decision-making process of the models.
- **Local Explainability:** **LIME (Local Interpretable Model-agnostic Explanations)** was applied to explain individual predictions, highlighting feature contributions for specific instances.

### 4. **Performance Evaluation**
- Comprehensive analysis of the trade-off between **model performance** and **time efficiency** before and after feature reduction.
- Demonstrated improvements in training and testing times with minimal impact on classification metrics.

## Datasets
- **NF-BoT-IoT-v2**
- **NF-ToN-IoT-v2**

These datasets were used to evaluate the performance of the IDS in identifying various attack types in IoT environments.

## Results
- Significant improvement in training/testing efficiency after feature reduction.
- Enhanced transparency and interpretability of the IDS using SHAP and LIME.

## How to Use
1. Clone the repository.
2. Preprocess the datasets as described in the preprocessing scripts.
3. Train and evaluate models using the provided machine learning pipelines.
4. Visualize explainability results using SHAP and LIME for both global and local insights.

## Citation
If you use this project in your research, please cite the relevant sources and this repository.

---

This project demonstrates the potential of combining high-performance machine learning models with explainability techniques to create transparent, efficient, and effective IDS solutions for IoT networks.
