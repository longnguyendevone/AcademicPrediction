# AcademicPrediction 

**Overview**

-   This project focuses on building a multi-class classification system to predict whether a university student will drop out, remain enrolled, or graduate.
    
-   It utilizes a comprehensive dataset from the UCI Machine Learning Repository containing 4,424 student records.
    
-   The dataset includes 36 distinct features categorized into demographic, socio-economic, academic background, academic performance, and macro-economic data.
    

**Methodology & Data Processing**

-   **Outlier Handling:** Applied the Winsorization technique using the Interquartile Range (IQR) to cap extreme values without deleting critical data points.
    
-   **Feature Selection:** Utilized Pearson correlation matrices for continuous variables and Chi-Square tests for categorical variables to eliminate redundant data and identify the most impactful predictors.
    
-   **Data Balancing:** Addressed the imbalance in the target variable by generating synthetic data points using the SMOTE-NC (Synthetic Minority Over-sampling Technique for Nominal and Continuous) algorithm.
    

**Model Architecture & Performance**

-   The project implements and compares a variety of machine learning models, including Naive Bayes, Decision Trees, Random Forests, XGBoost, LightGBM, and CatBoost.
    
-   To deeply understand algorithmic mechanics, hand-coded versions of several algorithms were built from scratch and benchmarked against their optimized library counterparts.
    
-   The optimized library version of **CatBoost** achieved the highest overall performance, reaching an accuracy of 75.82% and a Weighted F1-score of 0.76.
    
-   The optimized **LightGBM** model closely followed with an accuracy of 74.92%.
    
-   While hand-coded versions of Naive Bayes and Random Forest performed competitively with their library counterparts, the hand-coded Boosting algorithms (capped at 59.21% accuracy) were significantly outperformed by the specialized libraries.
