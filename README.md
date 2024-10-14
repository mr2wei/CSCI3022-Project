# Cook County Housing Data Analysis

## Overview

This project is a comprehensive analysis of housing data from Cook County, Illinois. The primary objective is to explore the dataset, perform exploratory data analysis (EDA), engineer features, and prepare the data for predictive modeling. The project is divided into two parts, with the first part focusing on data exploration and feature engineering, and the second part on building a predictive model.

## Project Structure

### Part 1: Exploratory Data Analysis and Feature Engineering

1. **Understanding the Dataset**:
   - Answering questions about the dataset and identifying key features for analysis.

4. **Exploratory Data Analysis (EDA)**:
   - Initial exploration of the dataset to understand the distribution and relationships between variables.
   - Used visualization techniques such as histplot, boxplot, and scatter plots to gain further insights into the data.

5. **Feature Engineering**:
   - The dataset is processed to extract any aditional information placed within columns such as 'Description'.
   - For example, the number of bedrooms is extracted from the `Description` column using regular expressions.

6. **Data Cleaning**:
   - The dataset is cleaned to handle missing values and outliers, ensuring the data is ready for modeling.

### Part 2: Predictive Modeling

1. **Data Preparation**:
   - Utilized a pipeline to process the data, ensuring consistent feature engineering across training and validation datasets.
   - Removed outliers by filtering rows where `Pure Market Filter` equals 0.
   - Applied log transformations to `Sale Price` and `Building Square Feet` to create `Log Sale Price` and `Log Building Square Feet`.

2. **Model Building**:
   - Implemented a linear regression model to predict housing prices based on the engineered features.
   - Split the data into training and validation sets to evaluate model performance.

3. **Model Evaluation**:
   - Assessed the model's accuracy using metrics such as Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE).
   - Analyzed residuals to ensure the model's assumptions were met and to identify any potential improvements.

4. **Advanced Techniques**:
   - Explored additional modeling techniques to enhance prediction accuracy, including regularization methods and ensemble models.
   - Compared the performance of different models to select the best approach for the dataset.
