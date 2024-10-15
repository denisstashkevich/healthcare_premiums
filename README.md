Healthcare Premium Prediction

This project aims to analyze healthcare premiums and build predictive models for individuals across different age groups. The goal is to understand the factors influencing healthcare premiums and develop accurate models to predict premium amounts. The project involves several key steps:

Data Loading and Cleaning: The dataset is loaded from an Excel file, and data cleaning operations are performed to ensure data quality. This includes handling missing values, removing duplicates, and correcting inconsistencies such as negative values for dependents and unrealistic ages.

Exploratory Data Analysis (EDA): EDA is conducted to understand the distribution of both numerical and categorical features. Techniques such as univariate and bivariate analysis, as well as visualizations like histograms, scatter plots, and box plots, are used to identify patterns, relationships, and outliers in the data.

Feature Engineering: Features are transformed and new features are created to enhance the predictive power of the model. This includes calculating a health risk score based on medical history, normalizing numerical features, encoding categorical features, and creating dummy variables for nominal categories.

Feature Selection and Multicollinearity Analysis: To improve model efficiency, irrelevant or redundant features are removed. Multicollinearity is checked using Variance Inflation Factor (VIF), and features with high VIF values are dropped to reduce redundancy.

Model Training: Various machine learning models are trained to predict healthcare premiums, including Linear Regression, Ridge Regression, and XGBoost. The dataset is split into training and testing sets, and models are evaluated based on metrics such as Mean Squared Error (MSE) and R-squared scores.

Hyperparameter Tuning: Hyperparameter tuning is performed using techniques like RandomizedSearchCV to optimize model performance, especially for complex models like XGBoost.

Error Analysis: Residual analysis is conducted to understand the prediction errors. Extreme errors are identified, and features contributing to these errors are analyzed. It is noted that a separate model might be required for certain demographics, such as younger individuals, to improve accuracy.

The overall objective is to improve the accuracy of premium predictions and provide insights into the key factors affecting healthcare costs.
