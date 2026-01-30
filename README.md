
# 🧠 Obesity Risk Factor Analysis

## 📌 Project Overview

This project analyzes **key demographic, behavioral, mental health, and lifestyle factors associated with obesity** among adults aged **20–65 years**. Using a multi-source public health dataset, the study focuses on understanding obesity risk drivers and building classification models to predict obesity categories **without directly using BMI or weight**, ensuring meaningful inference from underlying factors.

----------

## 🎯 Objectives

-   Identify major **risk factors contributing to obesity**
    
-   Perform **comprehensive data preprocessing and exploratory data analysis (EDA)**
    
-   Address **missing values and class imbalance**
    
-   Build and evaluate **machine learning classification models**
    
-   Predict obesity levels using **behavioral and demographic variables**
    

----------

## 📊 Dataset Description

The project integrates multiple datasets related to adult health indicators, including:

### Key Attributes

-   **Demographics**: Age, gender, race/ethnicity, income ratio
    
-   **Body Measures**: Height, weight, BMI
    
-   **Mental Health**: Depression indicators, appetite/overeating
    
-   **Sleep Patterns**: Weekday and weekend sleep duration
    
-   **Lifestyle Factors**: Smoking behavior
    

All datasets were merged using a unique respondent identifier.

### Source
CDC - National Center for Health Statistics. National Health and Nutrition Examination Survey March 2017 to 2020 Pre-pandemic.  
NHANES is a program of studies designed to assess the health and nutritional status of adults and children in the United States. The survey is unique in that it combines interviews and physical examinations.

----------

## 🛠️ Data Preprocessing

-   Renamed and standardized column names
    
-   Filtered population to **adults aged 20–65**
    
-   Dropped variables with excessive missingness (e.g., Smoking)
    
-   Handled missing values:
    
    -   **Mean imputation** for continuous variables
        
    -   **Mode imputation** for categorical variables
        
-   Corrected corrupted values caused by data import issues
    
-   Created **BMI-based obesity categories** using CDC guidelines
    
-   Removed **BMI and weight** from modeling to avoid data leakage
    

----------

## 📈 Exploratory Data Analysis

### Univariate Analysis

-   Distribution of demographic and lifestyle variables
    
-   Histograms and bar charts
    

### Bivariate Analysis

-   Scatter plots and box plots to observe relationships
    
-   Obesity distribution across demographic groups
    

### Multivariate Analysis

-   Correlation heatmap
    
-   Identified strong correlation between obesity, BMI, and weight
    

----------

## ⚖️ Handling Class Imbalance

-   Initial data showed dominance of **Overweight and Obese** categories
    
-   Re-grouped underrepresented classes
    
-   Achieved a more balanced target distribution to improve model performance
    

----------

## 🤖 Machine Learning Modeling

### Workflow

1.  Feature encoding for categorical variables
    
2.  Train–test split
    
3.  Feature scaling
    
4.  Model training and evaluation
    

### Models Used

-   Logistic Regression
    
-   Decision Tree Classifier
    
-   Random Forest Classifier 
-  K-NN
- Naive Bayes
- SVM
    

### Evaluation Metrics

-   Accuracy
    
-   Precision
    
-   Recall
    
-   F1-Score
    

----------

## 🧰 Tech Stack

-   **Python**
    
-   **Pandas, NumPy**
    
-   **Matplotlib, Seaborn**
    
-   **Scikit-learn**
    
-   **Jupyter Notebook**
    

----------

## 🚀 Key Insights

-   Obesity is strongly influenced by **sleep patterns and mental health indicators**
    
-   Removing BMI from modeling forces models to learn **true behavioral patterns**
    
-   Balanced data significantly improves classification reliability
