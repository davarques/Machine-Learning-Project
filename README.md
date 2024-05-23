# Machine Learning Project

<img src="https://datascientest.com/en/wp-content/uploads/sites/9/2021/01/Machine-learning-def-.png" alt="Machine Learning" width="800">

## Analyzing and Predicting Housing Market Trends using Supervised Machine Learning Models

## Project Overview 📋

This project utilizes a dataset containing house sale prices in King County, including Seattle, from May 2014 to May 2015. It mirrors real-world real estate analysis, encouraging collaborative problem-solving and practical application of Python in real estate finance.

## Goal 🎯

The goal of this project is to apply our Python and Machine Learning knowledge to:

1. **Analyze and clean the data**: Prepare the dataset by performing exploratory data analysis (EDA) and preprocessing steps such as handling missing values, removing outliers, and feature engineering.

2. **Apply different supervised regression machine learning models**: Utilize various regression algorithms such as linear regression, decision tree regression, random forest regression, etc., to train models on the cleaned dataset.

3. **Assess the results and choose the best model to deploy**: Evaluate the performance of each model using appropriate metrics like Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), etc. Select the most accurate and robust model for deployment in predicting house prices in the King County, Seattle market.

## Dataset 💾

- **Source**: [[Kaggle:] King County, Seattle House Market Price and Sources](https://www.kaggle.com/datasets/minasameh55/king-country-houses-aa)
- **Data Timeframe**: May 2014 to May 2015
- **Data Size**: (21613 rows, 21columns)

### Dataset Features:

- **`id`**: A unique identifier for each house.
- **`date`**: The date when the house was sold.
- **`price`**: The sale price of the house (prediction target).
- **`bedrooms`**: Number of bedrooms in the house.
- **`bathrooms`**: Number of bathrooms in the house per bedroom.
- **`sqft_living`**: Square footage of the interior living space.
- **`sqft_lot`**: Square footage of the land space.
- **`floors`**: Number of floors (levels) in the house.
- **`waterfront`**: Indicates whether the house has a waterfront view.
- **`view`**: Number of times the house has been viewed.
- **`condition`**: Overall condition of the house.
- **`grade`**: Overall grade given to the house based on the King County grading system.
- **`sqft_above`**: Square footage of the house apart from the basement.
- **`sqft_basement`**: Square footage of the basement.
- **`yr_built`**: The year the house was built.
- **`yr_renovated`**: The year the house was renovated.
- **`zipcode`**: ZIP code area.
- **`lat`**: Latitude coordinate.
- **`long`**: Longitude coordinate.
- **`sqft_living15`**: Interior living space for the nearest 15 neighbors in 2015.
- **`sqft_lot15`**: Land space for the nearest 15 neighbors in 2015.

**Target column:** `Price` Our primary focus is to understand which features most significantly impact house prices. Additionally, we aim to explore properties valued at $650K and above for more detailed insights.

## Exploratory Data Analysis 🔬

### EDA Insights

- The price data does not follow a normal distribution, indicating skewness towards lower prices.

![image](https://github.com/davarques/Machine-Learning-Project/assets/160759223/d89decc8-510e-4049-870a-43d2b60dc7ef)

- There is a high number of outliers with exceptionally high house prices, which could affect the model's performance if not addressed.

![Screenshot 2024-05-23 at 15 18 49](https://github.com/davarques/Machine-Learning-Project/assets/160759223/b07742b4-0ceb-4f02-a105-d34d40e37c42)

------------------------------------------------------------------------

## Machine Learning Models 🤖

In this porject we'll apply three regression supervised machine leraning models:

**Train-test Split = 70% Train / 30% Test**

<img src="https://github.com/davarques/Machine-Learning-Project/assets/160759223/82d402df-0362-4cf4-a089-c509b15849ca" alt="Screenshot 2024-05-23 at 15 57 09" width="650">

------------------------------------------------------------------------

## Results 📊

We got the following results: 

<img src="https://github.com/davarques/Machine-Learning-Project/assets/160759223/21ece455-b5ee-4109-b02c-3bf6c577f8f9" alt="Screenshot 2024-05-23 at 15 58 56" width="650">

------------------------------------------------------------------------

## Conclusion 🔎

Based on the evaluation metrics, the decision tree emerges as the best model for predicting accurate house sale prices in the Seattle (US) market. Here are the key findings:

- **Decision Tree R2**: 0.7366
- **Decision Tree RMSE**: 194996.9105
- **Decision Tree MSE**: 38023795092.7977
- **Decision Tree MAE**: 100868.8284

The decision tree model demonstrates the highest R2 score and the lowest RMSE, MSE, and MAE metrics among the models evaluated. Hence, it is the preferred choice for accurate predictions in this context.

