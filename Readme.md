# Breast Cancer Prediction Using Machine Learning Models

This repository contains an implementation of six machine learning models to predict breast cancer based on clinical and morphological data. Each model's performance was rigorously evaluated using **five-fold cross-validation**, ensuring robust and reliable results. This project demonstrates the use of machine learning techniques to tackle a critical medical problem and highlights the strengths and weaknesses of each model.

## Dataset

- The dataset used for this project contains breast cancer diagnostic features derived from clinical and morphological data.
- Features include measurements such as radius, texture, smoothness, and more.
- The target variable indicates whether a tumor is benign or malignant.

## Models Used

The following machine learning models were implemented for the classification task:

1. **Logistic Regression (LR)**
   - A simple yet powerful model for linear relationships.
   - Achieved the highest accuracy (0.977) and F1-Score (0.969) during five-fold cross-validation, showcasing robustness and reliability.

2. **Support Vector Machine (SVM)**
   - Excellent at handling complex and nonlinear patterns.
   - Delivered competitive results with an accuracy of 0.975 and F1-Score of 0.966, but computationally expensive.

3. **Random Forest (RF)**
   - An ensemble learning method reducing overfitting.
   - Achieved a balanced accuracy of 0.946 and F1-Score of 0.926, making it a reliable option for high-dimensional datasets.

4. **K-Nearest Neighbors (KNN)**
   - A distance-based algorithm.
   - Demonstrated strong predictive power (accuracy: 0.965, F1-Score: 0.952) but sensitive to scaling and computationally expensive for large datasets.

5. **Decision Tree (DT)**
   - Simple and interpretable but prone to overfitting.
   - Showed the lowest performance (accuracy: 0.903, F1-Score: 0.869), making it less suitable for complex datasets.

6. **Extreme Gradient Boosting (XGBoost)**
   - A powerful ensemble model for complex datasets.
   - Achieved balanced performance (accuracy: 0.958, F1-Score: 0.944) but required significant computational resources.

## Evaluation Methodology

To ensure the models' performance is not biased by the training/test split, **five-fold cross-validation** was applied. This method divides the dataset into five parts, with one part used as the test set and the remaining four as the training set, cycling through all five parts. The evaluation metrics include:

- Precision
- Recall
- F1-Score
- Accuracy

