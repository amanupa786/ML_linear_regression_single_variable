# Single Variable Linear Regression for House Price Prediction

## Overview
This project demonstrates **Single Variable Linear Regression** using **Scikit-Learn** to predict house prices based on area (square feet). The dataset (`home_prices.csv`) contains **house area and price data**, which we use to train a predictive model.

## Features
- Loads real-estate data (`home_prices.csv`).
- Builds a **Linear Regression model** to estimate house prices.
- Predicts prices for given **house sizes (sq ft)**.
- Extracts and interprets **model coefficients** (slope & intercept).
- Provides a **manual prediction formula** based on the trained model.

## Technologies Used
- **Python 🐍**
- **Pandas 📊**
- **Scikit-Learn 🤖**
- **Jupyter Notebook 📓**

## Dataset (`home_prices.csv`)
The dataset contains two columns:
1. **`area_sqr_ft`** - Size of the house in square feet.
2. **`price_lakhs`** - House price in lakhs.

### Sample Data:
| area_sqr_ft | price_lakhs |
|------------|------------|
| 656        | 39.0       |
| 1260       | 83.2       |
| 1057       | 86.6       |
| 1259       | 59.0       |
| 1800       | 140.0      |

## How It Works
1. **Load Dataset:** Reads `home_prices.csv`.
2. **Train Model:** Uses `LinearRegression` to fit a model on `area_sqr_ft` vs `price_lakhs`.
3. **Make Predictions:** Predicts house prices for new areas.
4. **Extract Coefficients:** Finds slope (`coef_`) and intercept (`intercept_`).
5. **Manual Price Calculation:** Uses the formula:
   
   ```math
   \text{Price} = (\text{Coefficient} \times \text{Area}) + \text{Intercept}
