# Canadian Employment Forecasting Using Machine Learning

### Predicting Employment Trends in the Construction and Mining Industries

## Project Overview

This project uses machine learning to predict monthly employment in selected Canadian industries using historical labour-market data.

The analysis focuses on:

- Construction
- Mining, quarrying, and oil and gas extraction

For each industry, two employee groups are analyzed:

- Employees paid by the hour
- Salaried employees paid a fixed salary

## Dataset

The project uses monthly Canadian employment and labour-market data containing:

- Employment
- Average hourly earnings
- Average weekly earnings
- Average weekly hours
- Industry
- Employee type

The data covers monthly observations from 2001 to 2026.

## Methodology

The project follows these steps:

1. Load and inspect the dataset
2. Clean and restructure the data
3. Perform exploratory data analysis
4. Create lagged features using historical employment and labour-market measures
5. Split the data chronologically into training and testing sets
6. Establish a baseline
7. Train Linear Regression and Ridge Regression models
8. Evaluate model performance using MAE, RMSE, and R²
9. Compare model performance across industries and employee types

## Models

- Baseline
- Linear Regression
- Ridge Regression

## Results

| Industry | Employee Type | Best Model | MAE |
|---|---|---|---:|
| Construction | Hourly | Linear Regression | 9,747.99 |
| Construction | Salaried | Ridge Regression | 7,983.59 |
| Mining | Hourly | Ridge Regression | 4,958.75 |
| Mining | Salaried | Linear Regression | 6,006.03 |

Lower MAE indicates better prediction performance.

## Key Findings

The results show that historical employment, earnings, and working-hours information can provide useful signals for predicting employment.

Model performance varied across industries and employee types. Ridge Regression performed best for Construction salaried employees and Mining hourly employees, while Linear Regression performed best for Construction hourly employees and Mining salaried employees.

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## Project Files

- `GOVT_CANADA_EMPLOYMENT_ANALYSIS.ipynb` — Complete analysis and machine learning workflow.
