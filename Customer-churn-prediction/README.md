# Customer Churn Prediction

A Python and machine learning project focused on analyzing telecom customer data and building models to predict customer churn.

## Project Overview

Customer churn occurs when customers discontinue a service. Understanding customer behavior and identifying factors associated with churn can help organizations analyze customer retention patterns.

This project uses the Telco Customer Churn dataset to perform data preparation, exploratory data analysis, regression, classification, and model evaluation.

## Problem Statement

The objective of this project is to analyze telecom customer data and build machine learning models to predict whether a customer will churn.

The target variable is:

`Churn`
- `Yes` — Customer churned
- `No` — Customer did not churn

The analysis uses customer attributes such as tenure, monthly charges, contract type, payment method, internet service, and other available customer information.

## Project Workflow

```text
Dataset
   ↓
Data Loading
   ↓
Data Understanding
   ↓
Data Cleaning
   ↓
Data Manipulation
   ↓
Exploratory Data Analysis
   ↓
Linear Regression
   ↓
Logistic Regression
   ↓
Decision Tree
   ↓
Random Forest
   ↓
Model Comparison
   ↓
Conclusion

```

## Dataset

The project uses the Telco Customer Churn dataset.

The dataset contains customer information including:

- Customer ID
- Gender
- Senior Citizen
- Partner
- Dependents
- Tenure
- Phone Service
- Multiple Lines
- Internet Service
- Online Security
- Online Backup
- Device Protection
- Tech Support
- Streaming TV
- Streaming Movies
- Contract
- Paperless Billing
- Payment Method
- Monthly Charges
- Total Charges
- Churn

## Data Preparation and Analysis

The project includes the following data preparation and analysis steps:

- Dataset shape and structure analysis
- Data type inspection
- Summary statistics
- Missing value identification and handling
- Duplicate record checking
- Removal of the customer ID from modeling
- Customer data filtering
- Churn distribution analysis
- Internet service distribution analysis
- Customer tenure distribution
- Tenure vs Monthly Charges analysis
- Tenure by Contract analysis
- Numerical outlier analysis
- Correlation analysis

## Machine Learning Models

### Linear Regression

Linear Regression is used to analyze relationships between numerical variables.

### Simple Linear Regression

 - Independent variable: Tenure
 - Dependent variable: Monthly Charges

### Multiple Linear Regression

 - Independent variables: Tenure and Monthly Charges
 - Dependent variable: Total Charges

The regression models are evaluated using Root Mean Squared Error (RMSE).

### Logistic Regression

Logistic Regression is used for customer churn classification.

### Simple Logistic Regression

 - Independent variable: Tenure
 - Dependent variable: Churn

### Multiple Logistic Regression
 - Independent variables: Customer attributes
 - Dependent variable: Churn

### Decision Tree

Decision Tree classification is used to predict customer churn.

### Simple Decision Tree

 - Independent variable: Tenure
 - Dependent variable: Churn

### Multiple Decision Tree

 - Independent variables: Customer attributes
 - Dependent variable: Churn

### Random Forest

Random Forest classification is used to predict customer churn.

### Simple Random Forest

 - Independent variable: Tenure
 - Dependent variable: Churn

### Multiple Random Forest

 - Independent variables: Customer attributes
 - Dependent variable: Churn

## Model Evaluation

The classification models are evaluated using:

 - Accuracy
 - Precision
 - Recall
 - F1-score
 - Confusion Matrix
 - Classification Report

Model accuracy is also compared across the classification approaches using the test dataset.

## Project Structure

```text
Customer-churn-prediction/
│
├── Data/
│   └── customer_churn.csv
│
├── Notebooks/
│   └── customer_churn_prediction.ipynb
│
├── README.md
└── requirements.txt

```

## Technologies Used

 - Python
 - Jupyter Notebook
 - NumPy
 - Pandas
 - Matplotlib
 - Seaborn
 - Scikit-learn

## Project Outcome

This project demonstrates a complete machine learning workflow for a customer churn prediction problem, covering data preparation, exploratory data analysis, model development, prediction, and evaluation.

The project applies multiple regression and classification techniques to analyze customer data and examine their performance on the churn prediction task.

## Future Improvements

The project can be extended into a more advanced machine learning and production-oriented solution by adding:

- Feature engineering
- Data preprocessing pipelines
- One-hot encoding
- Feature scaling where appropriate
- Handling class imbalance
- Hyperparameter tuning
- Cross-validation
- Additional machine learning algorithms
- Systematic model comparison
- Model deployment
- FastAPI
- Docker
- Automated testing
- CI/CD
- Cloud deployment
- Model monitoring

These improvements can be explored in a future advanced ML/MLOps version of the project.

## How to Run the Project

### 1. Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```
### 2. Navigate to the Project

```bash
cd Customer-churn-prediction
```
### 3. Create a Virtual Environment

```bash
python -m venv .venv
```

### 4. Activate the Virtual Environment

#### Windows

```bash
.venv\Scripts\activate
```

#### macOS/Linux

```bash
source .venv/bin/activate
```

### 5. Install Dependencies

```bash
pip install -r requirements.txt
```

### 6. Start Jupyter Notebook

```bash
jupyter notebook
```

Open:

`notebooks/customer_churn_prediction.ipynb`

Run the notebook cells from top to bottom.


## Author

### Devvarun Nagaram


