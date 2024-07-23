# CIND820-Project
This repository contains source code and related documents for the CIND820 Final Project course at Toronto Metropolitan University.

# Abstract
According to the American Cancer Society, breast cancer is the most commonly diagnosed cancer among women, with millions of new cases reported each year. Breast ccancer affects about one in eight women, making it one of the most prevalent and life-threatening cancers impacting females worldwide. Despite the advanced progress in early diagnosis, screening, and patient management, it is still the leading cause of cancer-related deaths among women. Recently, however, new studies have shown that 

Machine Learning (ML) approaches can aid in detecting breast cancer at an early stage and with high accuracy, allowing for increased survival rate because better treatment can be provided. Therefore, the objective of this study is to analyze the Breast Cancer Wisconsin (Diagnostic) dataset (WDBC) by applying various machine learning (ML) techniques to predict the presence of breast cancer, classifying tumor types, and identifying key features that influence diagnosis. The chosen theme is Predictive Analytics, with a focus on Classification.

The objective of this report is to find the of the attributes that have the largest impact on determining breast cancer (i.e., whether or not a tumor is benign or malignant). By using the Breast Cancer Wisconsin (Diagnostic) dataset (WDBC), a study on different classification approaches including: Logistic Regression (LR), Decision Tree (DT), and Naïve Bayes (NB), was conducted. The study concluded that the Logistic Regression classifier was the best classifier with the highest accuracy in comparison to the other two models. 

# Dataset
The data using for this project can be found as a csv file at (https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data) or on the original website here: https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic.

# Project Structure
01_abstract
Deliverables are contained on numbered folders. The abstract briefly describes the research question and methods that are used, while the  literature review provides a more in-depth break down of the project. 

02_data_review
The data review deliverable provides an overview of the data and the approach taken.

03_final_results
The final deliverable provides an overview of the data, approach, and regression.

# Results
The results of the analysis are summarized below.

569 cases were scraped, with 357 being benign and 212 categorized as Malignant. There were 33 columns and 569 rows. 23/33 features were selected for machine learning: 'radius_mean', 'texture_mean', 'smoothness_mean', 'compactness_mean','concavity_mean', 'concave points_mean', 'symmetry_mean', 'fractal_dimension_mean', 'radius_se', 'texture_se', 'smoothness_se','compactness_se', 'concavity_se', 'concave points_se', 'symmetry_se','fractal_dimension_se','texture_worst', 'smoothness_worst', 'compactness_worst', 'concavity_worst', 'concave points_worst', 'symmetry_worst', 'fractal_dimension_worst'. 

Binary logistic regression classifier, decision tree, and Gaussian Naive Bias classifers were fitted using a 70/30 split for training and test data.

The confusion matrix for each classification of the test cases is shown below.

**Logistic Regression:**
               precision    recall  f1-score   support

           0       0.99      0.97      0.98       108
           1       0.95      0.98      0.97        63

    accuracy                           0.98       171
   macro avg       0.97      0.98      0.98       171
weighted avg       0.98      0.98      0.98       171

**Decision Tree:**
               precision    recall  f1-score   support

      benign       0.97      0.95      0.96       108
   malignant       0.92      0.95      0.94        63

    accuracy                           0.95       171
   macro avg       0.95      0.95      0.95       171
weighted avg       0.95      0.95      0.95       171

**Naive Bayes:**
               precision    recall  f1-score   support

           0       0.94      0.94      0.94       108
           1       0.90      0.89      0.90        63

    accuracy                           0.92       171
   macro avg       0.92      0.92      0.92       171
weighted avg       0.92      0.92      0.92       171

## Conclusions
The level of effectiveness of the classification models was calculated with the number of correct and incorrect classification. The logistic regression model outperformed the other models. The performance metrics indicate a high level of effectiveness in classifying tumors. The model achieved an impressive accuracy of 0.98, demonstrating its strong capability in distinguishing between benign and malignant tumors.

The study also helped to identify the features that contribute to predicting breast cancer by using tree based classifiers. Application of data visualization and data analytics techniques, together with the application of data science tools, allowed the understanding of feature's predictive relevance.

For the future, it would be beneficial to train the models using the different features that were removed from the training set and compare/contrast how this helps or hinders the model's ability to predict accurately. 
