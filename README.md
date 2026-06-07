# House Price Prediction Using Advanced Machine Learning

## Project Overview

This project was completed as part of **Week 5 of the AnalystLab Africa Data Science Internship Program**. The objective was to build, evaluate, and compare multiple machine learning models for predicting house prices and to investigate the impact of hyperparameter tuning on model performance.

The project follows a complete machine learning workflow, including data preprocessing, model training, evaluation, performance comparison, and model optimization.

---

## Dataset

The dataset contains information about residential properties and their corresponding prices. Features include:

* Area
* Bedrooms
* Bathrooms
* Stories
* Main Road Access
* Guest Room Availability
* Basement Availability
* Hot Water Heating
* Air Conditioning
* Parking Spaces
* Preferred Area
* Furnishing Status

**Target Variable:**

* Price

Dataset Size:

* 545 Rows
* 13 Columns

---

## Project Workflow

### 1. Data Preprocessing

The following preprocessing steps were performed:

* Dataset exploration and inspection
* Duplicate checking
* Categorical variable encoding
* Feature scaling using StandardScaler
* Train-test split (80:20)

### 2. Baseline Model

A Linear Regression model was implemented as the baseline model for comparison.

### 3. Advanced Machine Learning Models

The following regression models were trained and evaluated:

* Linear Regression
* Decision Tree Regressor
* Random Forest Regressor
* Gradient Boosting Regressor
* Tuned Random Forest Regressor

### 4. Hyperparameter Tuning

GridSearchCV was used to optimize the Random Forest Regressor by tuning parameters such as:

* n_estimators
* max_depth
* min_samples_split

---

## Evaluation Metrics

The models were evaluated using:

* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)
* R² Score

---

## Results

| Model               |       MAE |      MSE |      RMSE | R² Score |
| ------------------- | --------: | -------: | --------: | -------: |
| Linear Regression   |   979,680 | 1.77E+12 | 1,331,071 |    0.649 |
| Decision Tree       | 1,231,069 | 2.73E+12 | 1,653,664 |    0.459 |
| Random Forest       | 1,006,680 | 1.90E+12 | 1,376,813 |    0.625 |
| Gradient Boosting   |   965,870 | 1.70E+12 | 1,304,636 |    0.663 |
| Tuned Random Forest | 1,042,644 | 2.09E+12 | 1,444,743 |    0.587 |

---

## Key Findings

* Gradient Boosting Regressor achieved the best overall performance.
* Decision Tree Regressor produced the weakest results.
* Ensemble learning methods outperformed a single Decision Tree.
* Hyperparameter tuning did not improve the Random Forest model in this case.
* The dataset contains nonlinear relationships that are effectively captured by boosting algorithms.

---

## Best Model

**Gradient Boosting Regressor**

Performance:

* MAE: 965,870
* RMSE: 1,304,636
* R² Score: 0.663

This model demonstrated the strongest predictive capability and provided the most accurate house price predictions.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## Repository Structure

```text
├── House_Price_Prediction.ipynb
├── Week5_House_Price_Report.docx
├── README.md
└── dataset.csv
```

---

## Conclusion

This project demonstrates the application of advanced machine learning techniques for regression problems. By comparing multiple models and applying hyperparameter tuning, it was possible to identify Gradient Boosting as the most effective model for house price prediction on this dataset. The project highlights the importance of model selection, evaluation, and optimization in building reliable predictive systems.
