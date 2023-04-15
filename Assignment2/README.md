# Electricity Usage Prediction Based on Weather Conditions

## Overview

The goal of this assignment is to develop a method to predict electricity usage based on weather conditions. Two datasets are provided for this task: weather data and energy usage data. Ensure the code is well-documented with comments and includes the exact sequence of operations needed to produce the resulting tables and figures.

## Data

1. **Weather**: Weather data for one year with daily weather conditions.
2. **Energy Usage**: Energy usage history for one year (in kW) with 30-minute intervals. The energy usage of specific devices like AC, Fridge, washer, etc., is also provided.

## Tasks

### 1. Data Examination and Merging
- Parse the time fields as necessary.
- Sum the energy usage (`use [kW]`) to get the per day usage.
- Merge the energy usage data with the weather data.

### 2. Data Splitting
- Split the merged data into training and testing sets.
- The goal is to predict the usage for each day in December using weather data.
- Drop the device-specific usage columns, retaining only the `use [kW]` column for prediction.
v
### 3. Linear Regression - Predicting Energy Usage
- Set up a simple linear regression model to train and predict daily energy usage for December using weather data features.
- Drop the `use [kW]` column in the test set before making predictions.
- Evaluate the model by calculating the Root Mean Squared Error (RMSE) using the original `use [kW]` column.
- Generate a CSV file of the predicted values with two columns: date and predicted value.

### 4. Logistic Regression - Temperature Classification
- Using weather data, classify daily temperatures as 'high' (>= 35) or 'low' (< 35).
- Set up a logistic regression model to classify temperatures for each day in December.
- Calculate the F1 score for the model.
- Generate a CSV file of the classification results with two columns: date and classification (1 for high, 0 for low).

### 5. Energy Usage Data Analysis
- Analyze the usage patterns of two devices during different times of the day.
  - Day: 6AM - 7PM
  - Night: 7PM - 6AM
- Determine if the washer is used only during the day and when the AC is used most.
- Plot these usage trends and explain the findings.

### 6. Visual Appeal and Layout
- Include explanations for all tasks where necessary.
- Document the procedure with suitable comments.
- Label all plots and include legends to enhance clarity.
- Adjust plot sizes and use appropriate color schemes to maximize readability.
- Compile everything in a Python notebook (`.ipynb`).

## Data
- The weather and energy usage datasets are provided along with this assignment.