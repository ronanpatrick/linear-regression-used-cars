# Used Cars: Simple Linear Regression 

## Overview
This activity applies Simple Linear Regression to predict the market price of a used car based on its mileage. A core focus of this exercise is practical data wrangling—specifically using regular expressions (regex) to clean string-based numerical data before training the machine learning model.

## Dataset
* **Source File:** `used_cars.csv`
* **Feature Used (X):** `milage` 
* **Target Variable (y):** `price`

## Tech Stack
* **Language:** Python
* **Data Preprocessing:** Pandas (Regex, Type Conversion)
* **Machine Learning:** Scikit-Learn (`linear_model.LinearRegression`)
* **Data Visualization:** Matplotlib

## Workflow & Methodology
1. **Data Wrangling (Regex):** The raw dataset contained strings with symbols (e.g., "$", ",", "mi"). I utilized Pandas string replacement with regex (`r'[$,mi.]'`) to strip these characters, handle missing `NaN` values, and successfully cast the columns to standard numeric types for modeling.
2. **Exploratory Visualization:** Plotted a scatter plot to visually inspect the inverse relationship between vehicle mileage and price.
3. **Model Training:** Fit a Simple Linear Regression model to find the line of best fit and establish the mathematical relationship (coefficient and intercept) between the two variables.
4. **Prediction:** Implemented a sample prediction to estimate the price of a vehicle with 100,000 miles.

## How to Run

### Option 1: Run in Cloud (Recommended)
You can view and run this notebook instantly in your browser using Google Colab:
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ronanpatrick/linear-regression-used-cars/blob/main/LINEAR_REGRESSION_used_cars.ipynb)

*(Note: To run the notebook in Colab, ensure you upload the `used_cars.csv` dataset to the session storage or update the pandas read path to the raw GitHub URL).*

### Option 2: Run Locally
1. Clone this repository: `git clone https://github.com/ronanpatrick/linear-regression-used-cars.git`
2. Install the required libraries: `pip install pandas scikit-learn matplotlib`
3. Open the `.ipynb` file in Jupyter Notebook or VS Code and run all cells.
