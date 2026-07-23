# Laptop Price Prediction

This Jupyter notebook demonstrates a machine learning workflow to predict laptop prices based on various specifications.

## Project Overview

The goal of this project is to build a regression model that can estimate the price of a laptop given its features such as screen size, RAM, storage, CPU, GPU, and operating system.

## Key Steps

1.  **Data Loading**: The `laptop_price.csv` dataset is loaded into a pandas DataFrame.
2.  **Data Preprocessing**: 
    -   Irrelevant columns are dropped.
    -   Categorical features like `TypeName`, `Cpu`, `OpSys`, and `Gpu` are one-hot encoded.
    -   Numerical features such as `ScreenResolution`, `Ram`, `Memory`, and `Weight` are extracted and converted to appropriate data types.
3.  **Exploratory Data Analysis (EDA)**: Basic data inspection and correlation analysis with the target variable (`Price_euros`) are performed.
4.  **Model Training**: 
    -   The data is split into training and testing sets.
    -   Features are scaled using `StandardScaler`.
    -   A `RandomForestRegressor` model is trained on the preprocessed data.
5.  **Model Evaluation**: The model's performance is evaluated using Root Mean Squared Error (RMSE) and visualized with a scatter plot of predicted vs. actual prices.

## Libraries Used

-   `pandas`
-   `numpy`
-   `matplotlib`
-   `seaborn` (for visualizations, though not explicitly used in the final notebook state, it's a common EDA tool)
-   `scikit-learn` (for preprocessing, model selection, and model training)

## How to Run

1.  Ensure you have all the necessary libraries installed (`pip install pandas scikit-learn matplotlib`).
2.  Place the `laptop_price.csv` file in the same directory as the notebook.
3.  Run all cells in the Jupyter notebook.
