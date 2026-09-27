# Customer Churn Prediction

## Project Overview

Customer churn is an important business problem for telecom companies. The goal of this project is to analyze customer data and build a machine learning model that predicts whether a customer is likely to churn.

This project uses the Telco Customer Churn dataset and follows a complete machine learning workflow:

- Data loading
- Data understanding
- Data cleaning
- Exploratory Data Analysis (EDA)
- Feature preparation
- Categorical encoding
- Train-test split
- Machine learning model training
- Model evaluation
- Model comparison

## Problem Statement

The objective of this project is to predict the Churn status of a telecom customer based on customer information, services, contract details, payment information, tenure, and charges.
The target variable is:

`Churn`

Possible values:

- `Yes`
- `No`

## Dataset

The project uses the Telco Customer Churn dataset.

The dataset contains customer information such as:

- Customer ID
- Gender
- Senior Citizen status
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
The dataset contains approximately 7,000 customer records.

## Project Structure

```text
customer-churn-prediction/
│
├── data/
│   └── customer_churn.csv
│
├── notebooks/
│   └── 01_customer_churn_prediction.ipynb
│
├── README.md
├── requirements.txt
└── .gitignore
```

## Folder Description

### data/

Contains the customer churn dataset.

### notebooks/

Contains the Jupyter Notebook used for data analysis, visualization, preprocessing, model training, and evaluation.

### README.md

Contains the project documentation.

### requirements.txt

Contains the Python libraries required to run the project.



## Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Machine Learning Workflow

The project follows these steps:

```text
Dataset
   ↓
Data Loading
   ↓
Data Understanding
   ↓
Data Cleaning
   ↓
Exploratory Data Analysis
   ↓
Feature Preparation
   ↓
Train-Test Split
   ↓
Model Training
   ↓
Model Evaluation
   ↓
Model Comparison

```

### 1. Data Loading

The dataset is loaded into a Pandas DataFrame using:

`pd.read_csv()`

The dataset is then inspected using:

- `head()`
- `shape`
- `info()`
- `describe()`
- `unique()`
- `value_counts()`

### 2. Data Cleaning

The following data-cleaning activities are performed:

#### TotalCharges Conversion

The TotalCharges column is converted from text/object format into numeric format.

`pd.to_numeric()`

Invalid values are converted into missing values using:

`errors="coerce"`

#### Missing Values

Missing values are identified and handled before model training.

#### Duplicate Records

Duplicate records are checked.

#### Customer ID

The customerID column is removed because it is an identifier and does not provide useful predictive information for the model.

### 3. Exploratory Data Analysis

Exploratory Data Analysis is performed to understand the dataset and identify patterns.

The analysis includes:

- Customer churn distribution
- Numerical feature analysis
- Categorical feature analysis
- Outlier analysis
- Correlation analysis
- Distribution visualizations

Visualizations are created using:

- Matplotlib
- Seaborn

### 4. Feature Preparation

Categorical variables are converted into numerical representations so that machine learning algorithms can process them.

The dataset is separated into:

`X` → Input features  
`y` → Target variable

where:

`X` = Customer information  
`y` = Churn

### 5. Train-Test Split

The dataset is divided into training and testing datasets.

The training dataset is used to train the machine learning models, while the testing dataset is used to evaluate their performance on unseen data.

### 6. Machine Learning Models

Three machine learning algorithms are explored in this project.

#### Logistic Regression

Logistic Regression is used as a classification model and provides a simple baseline for the churn prediction problem.

#### Decision Tree

Decision Tree is used to learn decision rules from customer features.

#### Random Forest

Random Forest is an ensemble machine learning algorithm that combines multiple decision trees to make predictions.

### 7. Model Evaluation

The trained models are evaluated using classification metrics.

The project includes evaluation using:

- Accuracy
- Confusion Matrix
- Classification Report

These metrics help understand how well the models classify customers into churn and non-churn categories.

### 8. Model Comparison

The performance of the different machine learning models is compared to understand how they perform on the customer churn prediction task.

The models compared are:

- Logistic Regression
- Decision Tree
- Random Forest

The comparison is based on the evaluation results obtained from the test dataset.

## Key Machine Learning Concepts Practiced

This project provides practical experience with:

- Classification
- Exploratory Data Analysis
- Data Cleaning
- Missing-value handling
- Categorical feature encoding
- Feature preparation
- Train-test splitting
- Logistic Regression
- Decision Trees
- Random Forest
- Model evaluation
- Confusion Matrix
- Classification Report
- Model comparison

## How to Run the Project

### 1. Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### 2. Navigate to the Project

```bash
cd customer-churn-prediction
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

`notebooks/01_customer_churn_prediction.ipynb`

Run the notebook cells from top to bottom.

## Project Outcome

The project demonstrates the complete basic machine learning workflow for a binary classification problem.

It starts with raw customer data and proceeds through data cleaning, exploratory analysis, feature preparation, model training, and model evaluation.

## Future Improvements

This project can later be upgraded into a production-oriented machine learning application by adding:

- Production preprocessing pipelines
- Better handling of class imbalance
- Additional evaluation metrics such as Precision, Recall, F1, ROC-AUC and PR-AUC
- Hyperparameter tuning
- XGBoost
- MLflow experiment tracking
- Model versioning
- FastAPI model serving
- Automated testing
- Docker
- CI/CD
- Cloud deployment
- Model and API monitoring

These improvements will form the next production/MLOps version of the project.

## Author

### Devvarun Nagaram

This project was created as part of a practical journey in Python and Machine Learning.

