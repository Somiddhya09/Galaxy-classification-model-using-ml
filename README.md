# Galaxy Classification using Machine Learning 🌌

![Status](https://img.shields.io/badge/Status-Completed-green)
![Model](https://img.shields.io/badge/Best%20Model-Random%20Forest-orange)
![Accuracy](https://img.shields.io/badge/Accuracy-89.5%25-brightgreen)

## 📌 Overview
This project classifies galaxies into **STARBURST** and **STARFORMING** subclasses using spectral and photometric data from the **Sloan Digital Sky Survey (SDSS)**. We addressed class imbalance and non-linear feature relationships to build a robust binary classifier.



[Image of galaxy classification types]


## 📂 Dataset
- **Source:** SDSS DR17 (100,000 samples).
- **Target:** `subclass` (Binary).
- **Features:** 39 inputs including Redshift, Flux, and Magnitudes (u, g, r, i, z bands).
- **Preprocessing:** Removed outliers, dropped IDs, and applied **Standard Scaling**.

## ⚙️ Models & Methodology
We evaluated five algorithms to find the best fit:
1.  **Logistic Regression** (Baseline)
2.  **Decision Tree**
3.  **K-Nearest Neighbors (KNN)**
4.  **Random Forest** (Ensemble)
5.  **Gradient Boosting**



[Image of random forest algorithm]


## 📊 Results
The **Random Forest Classifier** outperformed all other models, handling the class imbalance most effectively.

| Model | Accuracy | F1 Score |
| :--- | :--- | :--- |
| **Random Forest** 🏆 | **89.5%** | **0.894** |
| Gradient Boosting | 88.5% | 0.882 |
| Logistic Regression | 87.6% | 0.871 |
| KNN | 85.5% | 0.849 |
| Decision Tree | 84.9% | 0.849 |

## 🖼️ Visuals
*(Generated from the analysis)*
- **Class Distribution:** Highlights the prevalence of "Starforming" galaxies.
- **Redshift Distribution:** Shows distinct distance profiles for each class.
- **Model Comparison:** Bar chart verifying Random Forest's superiority.

## 🚀 Conclusion
**Random Forest** is the recommended model for this task, achieving **89.5% accuracy** and high precision/recall, making it suitable for automated astronomical classification.