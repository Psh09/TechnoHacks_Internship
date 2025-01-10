# Predicting Medical Insurance Costs: A Deep Dive into Healthcare Data

## Overview

In this project, we aim to predict medical insurance costs using personal attributes such as age, BMI, smoking habits, and region. The dataset used for this analysis is the "Medical Cost Personal Dataset" containing 1,338 records and 7 features. The goal is to uncover patterns that drive medical insurance charges and develop a model to predict them accurately.

## Dataset Overview

The dataset contains the following features:

- **age**: Age of the individual (18–64 years)
- **sex**: Gender (male, female)
- **bmi**: Body Mass Index (Body fat based on height and weight)
- **children**: Number of dependents covered by insurance
- **smoker**: Smoking status (yes, no)
- **region**: Residential region in the U.S. (northeast, northwest, southeast, southwest)
- **charges**: Medical insurance cost (target variable)

## Key Insights

- Smokers generally have significantly higher insurance charges.
- BMI has a notable impact on charges, with higher BMI resulting in higher medical costs.
- Medical costs increase with age, reflecting greater health risks.
- The Southeast region shows slightly higher medical costs than other regions.

## Steps Followed

1. **Data Preprocessing**: 
   - Categorical variables like sex, smoker, and region were encoded using One-Hot Encoding.
   - Multicollinearity was checked using the Variance Inflation Factor (VIF).
   - Features were standardized for model consistency.

2. **Exploratory Data Analysis (EDA)**:
   - Performed univariate and bivariate analysis to understand distributions and correlations.
   - Used log transformation to reduce the skewness of medical charges.

3. **Modeling**:
   - A baseline **Linear Regression** model was built.
   - A **Random Forest Regressor** was used with hyperparameter tuning via GridSearchCV to improve performance.

4. **Performance Metrics**:
   - **Linear Regression**: RMSE: 0.42, MAE: 0.27, R²: 0.80
   - **Random Forest Regressor** (after tuning): RMSE: 0.37, MAE: 0.20, R²: 0.85

5. **Cross-Validation**: RMSE (CV): 0.40 ± 0.06, confirming the model's generalization ability.

## Technologies Used

- **Python** (pandas, numpy, scikit-learn, seaborn, matplotlib)
- **Jupyter Notebook** for implementation
- **GridSearchCV** for hyperparameter tuning

## Conclusion

This project demonstrates how healthcare costs can be predicted using machine learning techniques. The Random Forest model, after hyperparameter tuning, significantly outperforms the baseline Linear Regression model, capturing complex patterns in the data. Smoking, BMI, and age were found to be the most important predictors of insurance charges.

## Future Work

- Explore more advanced models like Gradient Boosting or Neural Networks for potentially better accuracy.
- Incorporate external data sources such as geographical information to refine predictions.
- Investigate further feature engineering techniques to enhance model performance.

---


## License

This project is licensed under the MIT License.
