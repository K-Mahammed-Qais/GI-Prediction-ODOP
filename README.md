GI Tag Prediction System for ODOP Products
A Machine Learning–Based Classification and Interactive GUI Tool
1. Introduction

This project aims to analyze and predict the Geographical Indication (GI) status of products listed under India’s One District One Product (ODOP) initiative. The goal is to identify patterns in product characteristics and develop a predictive system using machine learning algorithms.

2. Objectives

To analyze ODOP product attributes such as product name, sector, category, and description.

To predict the GI eligibility ("Yes" or "No") using machine learning models.

To evaluate and compare the performance of multiple algorithms.

To design a GUI-based application for non-technical users to retrieve GI predictions easily.

3. Dataset Description

The dataset contains the following key fields:

State

District

Product Name

Category (Primary/Secondary/Tertiary)

Sector (Agriculture, Handicraft, Manufacturing, etc.)

Description

GI Status (Yes/No)

Ministry/Department

4. Data Preprocessing

Performed steps:

Removal of irrelevant columns (e.g., LGD Code, Photo).

Handling missing values.

Standardizing category and sector labels.

Cleaning text fields.

Creating combined text features.

Encoding categorical variables.

Creating numerical representations using TF-IDF vectorization.

5. Exploratory Data Analysis

EDA was carried out using:

Univariate plots — bar charts, pie charts

Bivariate plots — cluster bars, boxplots

Multivariate plots — bubble charts, stacked bars, cross-tab analysis

These analyses help understand the distribution of GI status across states, sectors, and categories.

6. Machine Learning Models Used

Five models were implemented:

Logistic Regression

Acts as the baseline classification model and helps interpret feature importance.

K-Nearest Neighbors (KNN)

Classifies based on similarity between product attributes.

Random Forest Classifier

An ensemble method that improves accuracy and reduces overfitting.

XGBoost Classifier

A boosting-based algorithm that achieved the highest accuracy (≈85%).

Support Vector Machine (SVM)

Creates optimized decision boundaries for classification.

7. Model Comparison
Model	Accuracy (%)
XGBoost Classifier	84.7%
Random Forest Classifier	81.1%
KNN	79.9%
SVM	78.7%
Logistic Regression	76.0%

XGBoost emerged as the best-performing model.

8. GUI Implementation

A Tkinter-based GUI was developed to:

Accept a product name as input

Retrieve matching records from the dataset

Display predicted GI status

Show results with color-coded labels (green for Yes, red for No)

Provide auto-suggestions for product names

This interface allows non-technical users such as policymakers and local entrepreneurs to access predictions easily.

9. Conclusion

The project successfully demonstrates that machine learning can effectively predict GI tag eligibility based on product attributes. It highlights key factors influencing GI certification and provides an easy-to-use tool for real-world application.

10. Future Scope

Integration of deep learning models like BERT for better text understanding.

Development of a web-based dashboard for broader accessibility.

Linking predictions with government ODOP portals to aid policy decisions.
