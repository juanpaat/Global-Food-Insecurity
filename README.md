# Global-Food-Insecurity


# Food Insecurity Prediction Using Machine Learning

## Overview

This repository contains the code, data, and documentation for a research project aimed at predicting global food insecurity using machine learning models. The study employs a variety of classification algorithms to identify countries that may require external food assistance based on key indicators such as food loss, forest change, access to drinking water, and the Human Development Index (HDI). This work seeks to support global food security initiatives by providing data-driven insights that can guide resource allocation and intervention planning.

## 1. Introduction

Food insecurity is a pressing global challenge, affecting millions of people worldwide. Predicting which countries will require external food assistance can aid governments, NGOs, and international organisations in proactively addressing potential food crises. This study leverages machine learning to build predictive models that can identify at-risk countries using historical data from the last 12 years, covering 139 countries. The objective is to create a reliable and interpretable model that can support decision-makers in understanding the factors contributing to food insecurity and taking preventive measures.

## 2. Methodology

### 2.1 Data Preprocessing and Exploratory Data Analysis (EDA)
- The dataset used in this research consisted of multiple indicators related to food security, including food loss percentage, forest cover change, access to clean drinking water, and HDI.
- The initial dataset underwent thorough preprocessing to handle missing values, standardise variable formats, and balance the class distribution using techniques such as Synthetic Minority Over-sampling Technique (SMOTE).
- Exploratory Data Analysis (EDA) was conducted to understand the distribution and relationships between variables, providing valuable insights into trends and correlations that could inform model building.

### 2.2 Model Building
- A range of classification algorithms were implemented, including Logistic Regression, Support Vector Machines (SVM), k-Nearest Neighbours (kNN), Decision Trees, Random Forest, Gradient Boosting, and Multi-layer Perceptron (Neural Networks).
- Hyperparameters were tuned using Random Search to find the optimal configuration for each model.
- The models were evaluated based on four key metrics: recall, precision, accuracy, and ROC_AUC. Special emphasis was placed on recall due to its importance in correctly identifying countries that need external assistance.

### 2.3 Model Evaluation
- **Recall** was prioritised as the main evaluation metric to minimise the number of false negatives, which represent countries that are in need of assistance but were not identified as such by the model.
- **Precision** and **ROC_AUC** were also analysed to ensure that models effectively reduced false positives and maintained a high level of class separation across varying decision thresholds.

## 3. Results and Analysis

The performance of the models varied across the different metrics, with Gradient Boosting and Random Forest emerging as the top performers. These models demonstrated high recall, precision, and ROC_AUC values, indicating their robustness in predicting food insecurity. The results are summarised as follows:

- **Gradient Boosting** achieved the highest recall of 0.978788 and a ROC_AUC of 0.975287, indicating its strong capability to identify true positive cases and distinguish between classes effectively.
- **Random Forest** showed comparable results, with a recall of 0.975758 and a ROC_AUC of 0.976907, making it an excellent alternative when interpretability is desired.
- **Decision Trees** and **Multi-layer Perceptron** also performed well, but were slightly less effective than the ensemble methods in terms of recall and ROC_AUC.
- **Logistic Regression** and **Support Vector Machines (SVM)** had lower recall and ROC_AUC scores, indicating that they were less effective in capturing the complexity of the data and distinguishing between the two classes.

The analysis suggests that ensemble methods like Gradient Boosting and Random Forest are the most suitable models for this context, balancing predictive power with reliability.

## 4. Conclusions

This research demonstrated the potential of machine learning models to predict food insecurity with high accuracy and reliability. By prioritising recall as the primary evaluation metric, the models were able to effectively identify countries that are at risk of food shortages, which is crucial for timely interventions. The results indicated that:

- **Gradient Boosting** and **Random Forest** should be prioritised in future studies and applications due to their strong performance across all evaluation metrics.
- Simpler models like **Decision Trees** can be useful for their interpretability, but may require ensemble techniques to improve predictive power.
- **Logistic Regression** and **SVM** are less effective for this particular task and should be used with caution unless the data is preprocessed differently or additional features are included.

The findings of this study have significant implications for global food security initiatives, providing a data-driven approach to proactively identifying at-risk countries. Future work could focus on integrating these models with real-time data and exploring other ensemble techniques to further enhance performance.


## 7. Contact Information

For any questions, feedback, or collaboration opportunities, please reach out to juanpabloalzatetamayo@gmail.com  .
