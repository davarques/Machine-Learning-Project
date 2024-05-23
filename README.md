# Machine Learning Project

<img src="https://datascientest.com/en/wp-content/uploads/sites/9/2021/01/Machine-learning-def-.png" alt="Machine Learning" width="800">

## Analyzing and Predicting Housing Market Trends using Machine Learning

## Project Overview 📋

This project utilizes a dataset containing house sale prices in King County, Seattle (US), from May 2014 to May 2015. The aim is to leverage our Python, EDA (Exploratory Data Analysis), and Machine Learning skills to analyze and predict house selling prices.

It simulates real-world real estate analysis, promoting collaborative problem-solving and the practical application of Python in real estate finance.

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

![Screenshot 2024-05-23 at 19 00 05](https://github.com/davarques/Machine-Learning-Project/assets/160759223/1d33975c-cf70-4165-a773-eb775ad64ddc)

------------------------------------------------------------------------

### `Price` Exploration

I divided the prices into 5 `price_ranks`: (<250k), (250k-500k), (500k-750k), (750k-1M), (>1M).

<img src="https://github.com/davarques/Machine-Learning-Project/assets/160759223/2e00be0d-f145-400b-9bda-a0ccd556a48b" alt="Machine Learning" width="600">

We can see that most of the house prices are within two rank prices (250k-500k ) & (500k-750k).

Then we looked at Boxplots by `price_rank`:

<img src="https://github.com/davarques/Machine-Learning-Project/assets/160759223/62fd1425-9ada-4251-aafb-436a647e51a7" alt="Machine Learning" width="600">

We observe that most of the outliers are within teh price rank of houses above 1M.

------------------------------------------------------------------------

## Machine Learning Models 🤖

In this porject we'll apply three regression supervised machine leraning models:

**Train-test Split = 70% Train / 30% Test**

<img width="730" alt="Screenshot 2024-05-23 at 18 21 15" src="https://github.com/davarques/Machine-Learning-Project/assets/160759223/0bbcfcbe-8ff6-4df1-bd3c-7e9e34b0d829">

------------------------------------------------------------------------

## Results 📊

We got the following results: 

<img src="https://github.com/davarques/Machine-Learning-Project/assets/160759223/21ece455-b5ee-4109-b02c-3bf6c577f8f9" alt="Screenshot 2024-05-23 at 15 58 56" width="750">

------------------------------------------------------------------------

## Conclusion 🔎

Based on the evaluation metrics, the <strong style="color:blue;">decision tree is the best model</strong> for predicting accurate house sale prices in the Seattle (US) market. Here are the key findings:

- **Decision Tree R2**: 0.7366
- **Decision Tree RMSE**: 194996.9105
- **Decision Tree MSE**: 38023795092.7977
- **Decision Tree MAE**: 100868.8284

The decision tree model demonstrates the <strong style="color:darkgreen;">highest R2</strong> score and the <strong style="color:red;">lowest RMSE, MSE</strong>, and MAE metrics among the models evaluated. Hence, it is the preferred choice for accurate predictions in this context.
