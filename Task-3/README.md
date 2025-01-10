# Car Insurance Premium Prediction - Linear Regression Model

## Overview

In this task, we aimed to predict car insurance premiums using a linear regression model. The goal was to uncover patterns in a dataset containing information about drivers and their car insurance premiums, such as driver age, experience, car age, and previous accidents, and build a predictive model to estimate the insurance premium based on these factors.

### Task Description:
- **Problem**: Build a linear regression model to predict car insurance premiums.
- **Steps**: 
  - Load and clean the data.
  - Conduct exploratory data analysis (EDA).
  - Engineer features to improve model performance.
  - Build and evaluate a linear regression model.

### Technologies Used:
- **Kaggle Notebook**: The project was carried out in a Kaggle notebook, leveraging its computational resources and ease of use for data science tasks.
- **Dataset**: The dataset used contains information about drivers, including factors such as driver age, experience, previous accidents, annual mileage, car age, and insurance premiums. It is publicly available on Kaggle.
- **Language**: Python was used for data analysis and model building, utilizing libraries such as Pandas, NumPy, Matplotlib, Seaborn, and Scikit-learn.
- **Model**: A linear regression model was built using the Scikit-learn library to predict the insurance premium.

### Results:
- The model was evaluated using **Mean Squared Error (MSE)** and **R-squared (R2)** metrics.
- The model performed well with an R2 score close to 1, indicating a high correlation between the features and the target variable (insurance premium).
- The evaluation showed that features like **Driver Age** and **Car Age** had the most significant influence on the insurance premium.

### Key Highlights:
- **Data Cleaning**: Missing values and data types were checked and appropriately handled.
- **Exploratory Data Analysis (EDA)**: Correlations between various features and the target variable were visualized.
- **Feature Engineering**: A new feature, "Driver Risk," was created based on the number of previous accidents and driver experience.
- **Model Building**: A simple linear regression model was trained, and its performance was evaluated using MSE and R2 scores.

### Conclusion and Future Work:
While the linear regression model provided a baseline for predicting insurance premiums, there is potential for improvement by experimenting with more complex models such as decision trees or ensemble methods. Future work could also involve incorporating additional data sources or performing hyperparameter tuning for better prediction accuracy.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
