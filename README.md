# 🚗 Car Insurance Prediction
## 📌 Context
This project analyzes annual car insurance data to understand customer behavior related to insurance claims.
The main objective is to identify patterns and features that influence whether a customer files a claim.
The dataset represents a realistic insurance scenario and is suitable for data analysis and machine learning tasks.
## 📊 Dataset Overview
- The dataset contains 19 columns:
  
    - 18 feature variables
    - 1 target variable
      
## 🎯Target Variable

- Outcome

   - 1 → Customer filed an insurance claim

   - 0 → Customer did not file an insurance claim

This problem is treated as a binary classification task.

## 🧹 Data Cleaning & EDA 
 - The dataset contained missing values, which were addressed using a data preprocessing pipeline to ensure clean and consistent data for analysis. After preprocessing, exploratory data analysis (EDA) revealed important patterns related to insurance risk.

**1. Outcome Distribution by Driving Experience Level**
<img width="571" height="321" alt="image" src="https://github.com/user-attachments/assets/419e4c41-88be-41e8-9695-d77d5136dd4e" />
 - High-risk customers (OUTCOME = 1) have a higher frequency of speeding violations, showing a strong link between traffic violations and risk.

**2.Credit Score Distribution by Outcome**
<img width="590" height="390" alt="image" src="https://github.com/user-attachments/assets/ee098e74-5175-477d-a9c5-938dfa325a51" />
- Low-risk customers (OUTCOME = 0) have higher median credit scores, indicating better financial stability reduces insurance risk.
  
**3. Speeding Violations Distribution by Risk Outcome**
<img width="517" height="416" alt="image" src="https://github.com/user-attachments/assets/bdfb3d92-7dee-46d2-807b-ccc784ce525e" />
- High-risk outcomes are most common among drivers with 0–9 years of experience, decreasing as experience increases.


## ⚖️ Class Imbalance Handling

- The target variable was not balanced in its raw form.

- Class balancing was performed during preprocessing to:

    - Reduce model bias toward the majority class

    - Improve generalization performance

    - Ensure fair evaluation of classification models

This makes the dataset more suitable for reliable machine learning experiments.


## 🧠 Feature Engineering

Several feature engineering strategies were explored:

- Using log-transformed features directly

- Feature Selection to retain the most informative variables

- PCA (Principal Component Analysis) for dimensionality reduction

These approaches were compared to evaluate their impact on model performance and overfitting.

## 🤖 Modeling Approach

The following methods were applied:

 - Random Forest Classifier

- PCA-based modeling

- Feature Selection–based modeling

**Key Findings:**

 - Random Forest and Feature Selection showed the best performance and generalization

 - PCA reduced dimensionality but resulted in some loss of predictive power

 - Model evaluation focused on train vs test performance to control overfitting

## 📈 Evaluation Strategy

- Train/Test split

- Accuracy comparison

 - Overfitting analysis

 - Performance comparison across different feature engineering techniques
 
## 💡 Insights & Inspiration

This project highlights:

- The importance of handling class imbalance in real-world datasets

- The impact of feature engineering on model performance

- How different dimensionality reduction techniques affect prediction quality

The dataset is well-suited for exploring **insurance risk modeling and customer behavior analysis.**
