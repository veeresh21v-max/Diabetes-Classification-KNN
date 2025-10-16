# Diabetes-Classification-KNN
# 🧬 Diabetes Classification using K-Nearest Neighbors (KNN)

## Project Overview

This project implements a Machine Learning workflow to classify whether a patient has Diabetes or not, based on various clinical and physical measurements. The **K-Nearest Neighbors (KNN)** algorithm is used, and the model is thoroughly preprocessed, tuned, and evaluated.

This project demonstrates skills in:
* Data Loading and Exploration (Pandas)
* Feature Scaling (StandardScaler)
* Model Selection and Hyperparameter Tuning (GridSearchCV, Cross-Validation)
* Handling Class Imbalance (Downsampling)
* Model Evaluation (Accuracy, Confusion Matrix)

## 📁 Repository Contents

* `Diabetes_Classification_KNN.ipynb`: The main Colab notebook containing all the Python code, analysis, and results.
* `README.md`: This documentation file.

## ⚙️ Dependencies and Environment

The entire project is designed to run seamlessly in **Google Colaboratory**. No local installation is required.

If running locally (using a Jupyter environment), the following Python libraries are required:
* `pandas`
* `numpy`
* `matplotlib`
* `seaborn`
* `scikit-learn` (`sklearn`)

## 🚀 How to Run the Project

1.  **Open the Notebook:** Click the "Open in Colab" badge below to launch the project directly in Google Colab.

    [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/15t5_48puDrIMxboJBppTU2cijHQpQv33?usp=sharing)

2.  **Run All Cells:** In the Colab menu, go to **Runtime** $\rightarrow$ **Run all**.

3.  **Explore Results:** The notebook will execute the entire workflow, including data preprocessing, hyperparameter tuning, and model evaluation, printing the best parameters, F-scores, and the final accuracy/confusion matrix.

## 📊 Key Findings

The model was trained on a dataset of patient health records sourced from IBM's Cognitive Class.

| Metric | Result |
| :--- | :--- |
| **Best $k$ (Neighbors)** | Determined via 10-fold cross-validation |
| **Best CV Accuracy** | Based on the tuned model |
| **Final Test Accuracy** | Accuracy on the held-out test set |

**Top Features (by F-Score):**
Feature selection revealed the following features as most impactful for the classification:
1.  **Glucose**
2.  **Cholesterol**
3.  **BMI**
4.  ... *(Check the F-Score table in the notebook for the full ranked list)*

## 💡 Project Steps

1.  **Data Acquisition:** Load the `Diabetes-Classification.xlsx` dataset from the remote source.
2.  **Feature Standardization:** Scale all numerical features using `StandardScaler`.
3.  **Class Imbalance Handling:** Downsample the majority class to balance the 'Diabetes' and 'No Diabetes' groups.
4.  **Model Training:** Train the KNN model on the scaled data.
5.  **Hyperparameter Tuning:** Use `GridSearchCV` to find the optimal number of neighbors ($k$).
6.  **Prediction and Evaluation:** Test the best model on the hold-out set and calculate accuracy and the confusion matrix.

---
*Developed as a college-level project for Machine Learning/Data Science.*
