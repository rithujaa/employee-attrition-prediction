# Employee Attrition Prediction

## Overview
This project predicts employee attrition in a corporate environment using machine learning techniques. By analyzing employee data, the project identifies key factors influencing attrition and builds predictive models to aid in decision-making.

## Dataset
- **Source**: IBM HR Analytics Dataset
- **Size**: 1,470 rows and 35 columns
- **Target Variable**: `Attrition` (`Yes` or `No`)

## Project Workflow
1. **Exploratory Data Analysis (EDA)**:
   - Examined feature distributions, correlations, and class imbalance.
   - Visualized key insights, such as the impact of `OverTime` and `JobSatisfaction`.

2. **Data Preprocessing**:
   - Encoded categorical variables using `LabelEncoder` and `One Hot Encoding`.
   - Addressed class imbalance using **SMOTE**.

3. **Modeling**:
   - Trained and evaluated the following models:
     - Logistic Regression
     - Random Forest
     - XGBoost
     - CatBoost
   - Used AUC, F1-score, and confusion matrices for performance evaluation.

4. **Results**:
   - **Best Model**: CatBoost with an AUC of **0.82** and balanced recall for both classes.
   - Identified key features such as `OverTime` and `JobSatisfaction` as strong predictors.

## Results Summary
| Model                | Precision | Recall | F1-Score | AUC  |
|----------------------|-----------|--------|----------|------|
| Logistic Regression  | 0.88      | 0.89   | 0.88     | 0.81 |
| Random Forest        | 0.82      | 0.84   | 0.82     | 0.76 |
| XGBoost              | 0.86      | 0.87   | 0.86     | 0.76 |
| CatBoost             | 0.84      | 0.83   | 0.83     | 0.82 |

