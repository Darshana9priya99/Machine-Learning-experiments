# Experiment 01: Polynomial Regression

## Objective

To implement Polynomial Regression on a real-world regression dataset and analyze the effect of different polynomial degrees on model performance.

## Dataset

**Energy Efficiency Dataset – UCI Machine Learning Repository**

The dataset contains 768 samples describing different building characteristics.

### Input Features

- X1 – Relative Compactness
- X2 – Surface Area
- X3 – Wall Area
- X4 – Roof Area
- X5 – Overall Height
- X6 – Orientation
- X7 – Glazing Area
- X8 – Glazing Area Distribution

### Target Variables

- Y1 – Heating Load
- Y2 – Cooling Load

In this experiment, **Heating Load (Y1)** is used as the target variable.

## Tasks Performed

1. Loaded and explored the Energy Efficiency dataset.
2. Performed Exploratory Data Analysis (EDA).
3. Checked dataset shape, columns, data types, missing values, and descriptive statistics.
4. Split the dataset into training and testing sets.
5. Applied Polynomial Regression for degrees 1 to 10.
6. Calculated MSE, RMSE, MAE, and R² for each degree.
7. Compared training and testing RMSE.
8. Identified underfitting and overfitting.
9. Selected the optimal polynomial degree.
10. Compared the best polynomial model with Linear Regression.

## Evaluation Metrics

- **MSE** – Mean Squared Error
- **RMSE** – Root Mean Squared Error
- **MAE** – Mean Absolute Error
- **R² Score** – Coefficient of Determination

## Results

The polynomial models were evaluated for degrees 1 to 10.

**Degree 5 produced the lowest testing RMSE and was selected as the optimal polynomial degree.**

| Model | Degree | RMSE | MAE | R² |
|---|---:|---:|---:|---:|
| Linear Regression | 1 | 3.0254 | 2.1821 | 0.9122 |
| Best Polynomial Regression | 5 | 0.4750 | 0.3552 | 0.9978 |

## Conclusion

Polynomial Regression significantly improved prediction performance compared with Linear Regression.

Degree 5 provided the best balance between model complexity and generalization. Lower-degree models showed comparatively higher errors, while increasing the polynomial degree beyond the optimal value increased testing error, indicating overfitting.

## Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

## Files

- `DarshanaPriya_ML_Experiment1_PolynomialRegression.ipynb` – Complete implementation
- `ENB2012_data.xlsx` – Energy Efficiency dataset
