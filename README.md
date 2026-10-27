# Regional Retail Revenue Predictor

## Project Overview
This repository contains the code and findings for the Data Science Internship project at Next Gen Software Hub Pvt. Ltd. The primary objective of this project is to analyze retail data and build a basic Machine Learning model to predict sales revenue based on regional and categorical features. 

## Dataset
The project utilizes the **Kaggle Superstore Sales dataset**. The dataset contains transaction-level data, including information such as `Region`, `Category`, `Row ID`, `Postal Code`, and our continuous target variable, `Sales`. 

## Approach & Methodology

The project was divided into four core phases:

### Week 1: Environment Setup & Python Basics
* Initialized the workspace using Jupyter Notebook.
* Implemented foundational Python concepts including conditional statements (`if/elif/else`), loops, and custom functions to simulate basic retail logic and conversion rates.

### Week 2: Data Handling (Pandas & NumPy)
* Loaded the CSV dataset using the Pandas library.
* Handled basic data manipulation tasks, including filtering high-performing sales, sorting data in descending order, and grouping total sales by region to identify geographical performance.

### Week 3: Exploratory Data Analysis (EDA)
* Cleaned the dataset by dropping missing values to ensure modeling accuracy.
* Utilized **Matplotlib** and **Seaborn** to visualize trends:
  * Plotted the spread of `Sales` across transactions (`Row ID`).
  * Generated a correlation matrix (heatmap) for the available numerical columns (`Row ID`, `Postal Code`, and `Sales`) to check for underlying relationships prior to modeling.

### Week 4: Machine Learning (Scikit-Learn)
* **Feature Engineering:** Since the primary numerical features were limited, categorical variables (`Category`, `Region`) were converted into numeric dummy variables to train the model.
* **Data Splitting:** Divided the dataset into training (80%) and testing (20%) sets.
* **Modeling:** Implemented a **Linear Regression** model using Scikit-Learn to predict `Sales`. 

## Results and Outputs
The model successfully processed the engineered features to output revenue predictions. By comparing the predicted sales against the actual sales in the test set, an R-squared score was generated that evaluates the variance captured by the regional and categorical predictors. *

## Technologies Used
* Python 3
* Jupyter Notebook / Google Colab
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-Learn