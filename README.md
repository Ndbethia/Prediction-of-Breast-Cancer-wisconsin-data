# Prediction-of-Breast-Cancer-wisconsin-data
# Introduction
This a prediction of the type of cancer either benign or malignant a lady can develop based on different variables.

The dataset was gotten from Kaggle for a project to sharpen our Python, Machine learning skills using googlecolab. The datasets gives a breakdown of breast cancer reports and categories 'B' Benign cancer, 'M' Malignant cancer with a 569 rows and 33 columns, the datasets consist of both numerical and categorical data.

# Data Analysis
we imported our libraries and models for analysis, we romoved null values and fixed missing values and errors then we performed 
*label encoding and one hot encoding to transform categorical variables to numerical variables (dummy_variables) for us to do further analysis like training and testing our datasets for predictions.

 ![image](https://github.com/user-attachments/assets/ef0aaa68-32ad-43af-98a8-9715b0738c35)

 # Correlation Analysis 
 performed correlation analysis to show relationships between the features 

 ![image](https://github.com/user-attachments/assets/bca19262-23c5-4eda-bd7d-9983b84a6370)

Visualized the distribution of the data features of cancer 
![image](https://github.com/user-attachments/assets/d9e37f83-fb27-4a2b-8308-e3f09407d922)
![image](https://github.com/user-attachments/assets/67897022-2e32-4020-adb1-c38b1f91d760)

The histograms are color-coded based on the diagnosis ('M' for malignant and 'B' for benign). This allows us to compare the distributions of features between malignant and benign diagnoses. We can observe that there are noticeable differences in the feature distributions between the two diagnoses.

By examining the histograms, we can identify features that exhibit distinct distributions for malignant and benign diagnoses. Features that show clear separation or significant differences in their distributions between the two diagnoses may be potential discriminative factors for distinguishing between malignant and benign cases.

Features with distributions that vary significantly between diagnoses may have higher predictive power i.e radius_mean, texture_mean, perimeter_mean, area_mean, compactness_mean, concavity_mean and so on


![image](https://github.com/user-attachments/assets/cdcc038b-7fbb-430e-a4b7-264de644b5b5)

# MACHINE LEARNING - SVM
SVM can be applied to improve the accuracy of medical condition diagnosis in the following ways:

# Optimizing SVM Parameters: 
Using techniques like grid search can improve model performance. By tuning parameters such as regularization parameter, kernel type and kernel specific parameters, the best configuration can be found.
Handling Class Imbalance: Usinf class-weighted SVMs can help address overfitting/underfitting and improve the model's ability to correctly classify classes.
Preprocessing and Normalization: Preprocessing techniques such as scaling and normalization can imporve the SVM performance by ensuring that all features have a similar scale hence improving convergence.
Model Interpretability: SVMs provide interpretable decision boundaries, making it easy to understand the reasoning behind the models predictions.

![image](https://github.com/user-attachments/assets/8707d48e-824c-443f-af1a-301634fabb64)

![image](https://github.com/user-attachments/assets/9bd0cd6f-2a2a-4754-8b47-c2063d519f4c)
# MODEL PARAMETER OPTIMIZATION
Use Scikit-learn's GridSearchCV to perform the grid search. It automatically trys out all combinations of parameter values. Afterwards, the best combination of parameters is used to create the SVM model

![image](https://github.com/user-attachments/assets/51293d32-8436-44d5-be4e-166d51d733d3)

![image](https://github.com/user-attachments/assets/b15856d6-32b6-4806-a7cb-fed25b84b846)






