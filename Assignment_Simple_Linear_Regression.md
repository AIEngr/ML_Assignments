# **Simple Linear Regression Analysis of Delivery Logistics**

This project demonstrates the application of **Simple Linear Regression** to predict delivery costs based on distance using a logistics dataset.

## **Project Overview**

The goal of this analysis is to model the linear relationship between the independent variable (**distance in km**) and the target variable (**delivery cost**). By training a model on historical data, we can accurately estimate the cost of a delivery given its distance.

## **Dataset Description**

- **Source File:** `Delivery_Logistics.csv`.
- **Initial Scale:** The raw dataset contains **25,000 rows and 15 columns**.
- **Practice Set:** For the core analysis and visualization, a subset of **20 random samples** was extracted to ensure consistency and clarity.
- **Key Features:**
    - `distance_km`: The total distance of the delivery.
    - `delivery_cost`: The associated cost for the delivery.

## **Technical Stack**

The following Python libraries were utilized for data processing, visualization, and machine learning:

- **Pandas & NumPy:** For data manipulation and numerical operations.
- **Matplotlib & Seaborn:** For generating scatter plots and regression line visualizations.
- **Scikit-Learn:** Specifically the `linear_model.LinearRegression` class for training the predictive model.

## **Workflow**

1. **Data Ingestion:** Loading the dataset and inspecting its initial shape and column types.
2. **Exploratory Data Analysis (EDA):** Checking for null values and visualizing the raw data points using a **Seaborn scatter plot**.
3. **Feature Selection:** Isolating the two continuous numeric columns (`distance_km` and `delivery_cost`) required for Simple Linear Regression.
4. **Model Training:** Fitting the `LinearRegression` model to the 20-row practice dataset.
5. **Prediction & Verification:** Testing the model with a sample distance (237.3 km) and manually verifying the output using the linear equation formula: $y = mx + b$.

## **Model Performance & Insights**

The model demonstrated high predictive accuracy based on the following metrics:

- **R-Squared Score:** **0.9716**, indicating that approximately **97.16%** of the variance in delivery cost is explained by distance.
- **Coefficient (Slope):** **~5.099**. This means for every 1 km increase in distance, the delivery cost increases by approximately **$5.10**.
- **Intercept:** **~136.18**. This represents the base cost of a delivery even when the distance is zero.

## **Visualizations**

The project includes clear visual evidence of the model's effectiveness:

- **Scatter Plot:** Shows the actual distribution of delivery data.
- **Regression Line:** Overlays a red "line of best fit" to demonstrate the strong positive correlation between distance and cost.
