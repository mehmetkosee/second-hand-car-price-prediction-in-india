# Second Hand Car Price Prediction

This project focuses on predicting the selling price of second-hand cars using various machine learning algorithms. The dataset includes information about cars such as year, present price, kilometers driven, fuel type, seller type, and transmission type.

## Project Overview

The goal of this project is to build a regression model that can accurately estimate the selling price of a used car based on its features. The workflow includes data preprocessing, exploratory data analysis, model training, and evaluation.

Three different regression models were implemented and compared:
1. Linear Regression
2. Random Forest Regressor
3. XGBoost Regressor

## Dataset

The dataset used in this project contains the following features:

- **Car_Name**: Name of the car
- **Year**: Year of purchase
- **Selling_Price**: Selling price of the car (Target Variable)
- **Present_Price**: Current ex-showroom price of the car
- **Kms_Driven**: Total kilometers driven
- **Fuel_Type**: Fuel type of the car (Petrol, Diesel, CNG)
- **Seller_Type**: Type of seller (Dealer, Individual)
- **Transmission**: Transmission type (Manual, Automatic)
- **Owner**: Number of previous owners

## Technologies Used

- Python 3
- Pandas (Data manipulation)
- NumPy (Numerical computations)
- Scikit-learn (Machine learning models and metrics)
- XGBoost (Gradient boosting framework)
- Matplotlib & Seaborn (Data visualization)

## Methodology

1. **Data Preprocessing**: 
   - Checked for missing values.
   - Performed One-Hot Encoding for categorical variables (Fuel_Type, Seller_Type, Transmission).
   - Split the data into features (X) and target (y).
   - Split the dataset into training (80%) and testing (20%) sets.

2. **Model Training**: 
   - Trained Linear Regression, Random Forest, and XGBoost models.

3. **Evaluation**: 
   - Evaluated models using Root Mean Squared Error (RMSE) and R-squared (R2) score.

## Results

The performance of the models on the test set is summarized below:

| Model | RMSE | R2 Score |
|-------|------|----------|
| Linear Regression | 1.87 | 0.85 |
| **Random Forest** | **0.88** | **0.97** |
| XGBoost | 1.01 | 0.96 |

**Random Forest Regressor** achieved the best performance with an R2 score of 0.97 and the lowest RMSE.

## Feature Importance

Based on the Random Forest model, the most important features determining the car price are:

1. **Present_Price** (Most dominant factor)
2. **Year** (Vehicle age)
3. **Kms_Driven**
4. **Transmission** (Manual vs Automatic)

## License

This project is open-source and available for educational purposes.
