# Laptop Price Predictor

## Problem Statement
The goal of this project is to predict the price of laptops based on various attributes such as brand, processor, RAM, storage, screen size, and other features. By building a predictive model, this project aims to assist potential buyers in estimating the price of laptops based on their specifications, helping them make more informed decisions.

## About Dataset
The dataset used for this project contains information about different laptops, including their specifications and prices. Key features in the dataset include:
- **Brand**: The manufacturer of the laptop.
- **Processor**: The type of processor in the laptop (e.g., Intel, AMD).
- **RAM**: The amount of memory in the laptop (in GB).
- **Storage**: The storage capacity (in GB).
- **Screen Size**: The size of the laptop screen (in inches).
- **Price**: The price of the laptop (target variable).

The dataset is used to train a machine learning model that predicts the price based on the provided features.

## Overall Analysis and Prediction
### Data Preprocessing
- Cleaned the dataset by handling missing values and encoding categorical variables.
- Split the dataset into training and testing sets for model evaluation.
  
### Feature Engineering
- Selected relevant features such as **Brand**, **Processor**, **RAM**, **Storage**, and **Screen Size** for model training.
  
### Model Development
- Used regression algorithms like **Linear Regression** and **Random Forest Regressor** to train the model.
- Evaluated the models using performance metrics such as **Root Mean Squared Error (RMSE)** and **Mean Absolute Error (MAE)**.

### Predictions
- The model predicts the price of a laptop based on its features, which can be used for real-time predictions when a new set of features is provided.
  
### Example Use Case
```python
# Example to predict laptop price
features = [8, 'Intel', 512, 15.6, 'HP']  # Example input for features: RAM, Processor, Storage, Screen Size, Brand
predicted_price = model.predict([features])
print("Predicted Price:", predicted_price)
