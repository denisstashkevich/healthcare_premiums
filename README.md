# Insurance Annual Premium Analysis and Prediction

<h2 align="center" style="color:blue">Project Description</h2>

This project focuses on analyzing insurance premium data and building models to predict the **annual premium amount**. We utilize various data cleaning methods, Exploratory Data Analysis (EDA), feature engineering, and machine learning models, including Linear Regression, Ridge, Lasso, and XGBoost.

<h2 align="center" style="color:blue">Project Structure</h2>

1. **Data Loading**
2. **Exploratory Data Analysis and Cleaning**
    - Handling Missing Values
    - Removing Duplicates
    - Cleaning Numerical and Categorical Features
    - Outlier Analysis
3. **Feature Engineering**
    - Creating New Features
    - Encoding Categorical Variables
    - Feature Selection and Multicollinearity Check
4. **Model Building**
    - Linear Regression
    - Ridge Regression
    - XGBoost Regression
5. **Model Evaluation and Results Analysis**
    - Model Performance Metrics
    - Residual Analysis
    - Identifying Extreme Errors

<h2 align="center" style="color:blue">Technologies and Libraries</h2>

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- statsmodels
- XGBoost

<h2 align="center" style="color:blue">Installation</h2>

1. **Clone the Repository:**

    ```bash
    git clone https://github.com/yourusername/insurance-premium-prediction.git
    cd insurance-premium-prediction
    ```

2. **Create and Activate a Virtual Environment (Optional):**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

3. **Install Required Dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

<h2 align="center" style="color:blue">Usage</h2>

1. **Data Preparation:**

    Ensure that the `premiums.xlsx` file is located in the root directory of the project.

2. **Run Jupyter Notebook:**

    ```bash
    jupyter notebook
    ```

    Open the `Insurance_Premium_Prediction.ipynb` file and follow the steps for data analysis and model building.

<h2 align="center" style="color:blue">Data Description</h2>

- **age**: Age of the insured individual.
- **income_lakhs**: Annual income in lakhs.
- **number_of_dependants**: Number of dependents.
- **gender**: Gender.
- **region**: Region of residence.
- **marital_status**: Marital status.
- **bmi_category**: Body Mass Index category.
- **smoking_status**: Smoking status.
- **employment_status**: Employment status.
- **income_level**: Income level.
- **medical_history**: Medical history.
- **insurance_plan**: Insurance plan.
- **annual_premium_amount**: Annual premium amount (target variable).

<h2 align="center" style="color:blue">Methodology</h2>

1. **Data Loading and Preprocessing:**
    - Import libraries.
    - Load data from Excel.
    - Clean column names (convert to lowercase and replace spaces with underscores).

2. **Exploratory Data Analysis (EDA):**
    - Analyze missing values and duplicates.
    - Statistical description of data.
    - Handle anomalies and outliers in `age` and `income_lakhs` features.
    - Visualize distributions and relationships between features.

3. **Feature Engineering:**
    - Create `total_risk_score` based on medical history.
    - Normalize the risk score.
    - Encode categorical variables using one-hot encoding.
    - Feature selection and removal of multicollinear features with high VIF.

4. **Model Building and Evaluation:**
    - Split data into training and testing sets.
    - Train Linear Regression, Ridge, and XGBoost models.
    - Evaluate models using R², MSE, and RMSE metrics.
    - Hyperparameter tuning for XGBoost using RandomizedSearchCV.
    - Analyze feature importance and residuals.

<h2 align="center" style="color:blue">Results</h2>

- **Linear Regression:**
    - Model coefficients visualized to understand the impact of each feature.
    - Performance metrics: R², MSE, RMSE.

- **Ridge Regression:**
    - Improved performance metrics compared to Linear Regression due to regularization.

- **XGBoost Regression:**
    - Best performance metrics after hyperparameter tuning.
    - Feature importance displayed for model interpretation.
    - Residual analysis identified 30% extreme errors associated with specific customer segments.

<h2 align="center" style="color:blue">Conclusion</h2>

The project demonstrates a complete data analysis and modeling pipeline for predicting insurance premiums. Key factors influencing the premium amount were identified, and model errors were analyzed, suggesting potential improvements such as building separate models for specific customer segments.

<h2 align="center" style="color:blue">Future Work</h2>

- Develop specialized models for segments with high error rates.
- Implement more advanced outlier and anomaly detection methods.
- Explore additional data sources to enhance prediction accuracy.
- Automate the model building and deployment process.

<h2 align="center" style="color:blue">Contact</h2>

