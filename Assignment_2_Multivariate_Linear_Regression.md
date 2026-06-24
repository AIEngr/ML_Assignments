**2. Multivariate Linear Regression: Medical Insurance Charges Prediction**

**Project Overview**

This assignment extends linear modeling into **Multivariate Linear Regression**. The project predicts medical insurance costs by analyzing a combination of demographic and lifestyle factors, demonstrating how multiple features interact to influence a single target variable.

- **Objective:** Predict the **log-transformed insurance charges** based on three features: `age`, `bmi`, and `is_smoker`.
- **Dataset:** `insurance.csv` (1,338 records).
- **Key Technical Features:**
    - **Feature Engineering:** Converting categorical 'smoker' status into a boolean `is_smoker` variable.
    - **Target Transformation:** Using `log_charges` to normalize the distribution of insurance costs for better model fit.
    - **Data Splitting:** 75/25 Train-Test split to evaluate model generalization.
- **Model Performance:**
    - **R-Squared Score (Testing):** 0.7502.
    - **Learned Weights:** Smoker status (2.23) has the highest impact, followed by Age (0.0489) and BMI (0.0152).
