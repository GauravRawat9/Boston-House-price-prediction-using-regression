# Boston-House-price-prediction-using-regression
This project focuses on predicting house prices using the Boston Housing dataset through multiple regression techniques, feature analysis, and model improvement strategies.

📌 Project Objective

To build and compare multiple regression models to predict MEDV (Median Home Value) using socioeconomic and housing-related features such as:

CRIM – Crime rate
RM – Average number of rooms
LSTAT – % lower status population
NOX – Nitric oxide concentration
TAX – Property tax rate
PTRATIO – Pupil-teacher ratio
And more

The goal was to:
Perform Exploratory Data Analysis (EDA)
Identify key correlated features
Build baseline and improved regression models
Compare performance using RMSE, R², and residual diagnostics

📊 Exploratory Data Analysis (EDA)

Checked dataset shape, info, and missing values
Performed correlation analysis
Visualized feature relationships using:
Correlation heatmap
Scatter plots (RM vs MEDV, LSTAT vs MEDV)

Key Observations:

RM (rooms) shows strong positive correlation with price
LSTAT shows strong negative correlation
Multicollinearity present among some features

🤖 Models Implemented
1️⃣ Linear Regression (Baseline Model)

Trained using all features
Evaluated using:
R² Score
RMSE
MSE

Visualized:
Predicted vs Actual values
Residual plots

2️⃣ Ridge Regression (Regularization)

Used to reduce overfitting and multicollinearity
Hyperparameter tuning with RidgeCV
Improved generalization performance compared to vanilla Linear Regression

3️⃣ Log Transformation + Scaling

Applied log transform to target variable (log1p(MEDV))
Standardized features using StandardScaler
Reduced skewness and improved model stability

4️⃣ Random Forest Regressor

Implemented ensemble model
Compared training and testing performance
Observed better handling of nonlinear relationships

📈 Evaluation Metrics

R² Score
RMSE (Root Mean Squared Error)
MSE (Mean Squared Error)
Residual analysis for model diagnostics

🛠 Tech Stack

Python
NumPy
Pandas
Matplotlib
Seaborn
Scikit-learn

🚀 Key Learnings

Feature correlation plays a critical role in regression performance
Regularization helps combat multicollinearity
Log transformation improves stability when target distribution is skewed
Ensemble models can outperform linear models for nonlinear relationships
Residual diagnostics are essential for validating regression assumptions

🔮 Future Improvements

Add cross-validation
Hyperparameter tuning for Random Forest
Feature selection using Lasso
Try Gradient Boosting / XGBoost
Deploy model using Flask or FastAPI
