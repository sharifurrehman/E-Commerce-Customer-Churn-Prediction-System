# 🚀 E-Commerce Customer Churn Prediction System

## 📌 Project Overview

The E-Commerce Customer Churn Prediction System is an end-to-end machine learning project that predicts whether an e-commerce customer is likely to leave a business using a **Random Forest Classifier**.

This project analyzes customer information, shopping preferences, satisfaction levels, complaints, and other available attributes to identify patterns associated with customer churn.

The goal is to help businesses understand customer behavior and support data-driven customer retention strategies.

## 🎯 Project Objectives

- Analyze customer data using Exploratory Data Analysis (EDA).
- Automatically download and load the dataset.
- Handle duplicate records and missing values.
- Prepare numerical and categorical features.
- Train a Random Forest classification model.
- Evaluate the model using multiple classification metrics.
- Visualize the confusion matrix and ROC curve.
- Identify important predictive features.
- Generate customer churn probabilities and risk categories.

## 📊 Dataset

**Dataset:** E-Commerce Customer Churn Analysis and Prediction

**Sources:**

- [Kaggle Dataset](https://www.kaggle.com/datasets/ankitverma2010/ecommerce-customer-churn-analysis-and-prediction)
- [Public GitHub Dataset Mirror](https://github.com/Leangonplu/Ecommerce_Customer_Churn_Analysis_and_Prediction)

The notebook automatically downloads the Excel dataset from the public GitHub mirror.

**Target variable:** `Churn`

- `0` — Customer retained
- `1` — Customer churned

The notebook inspects the dataset columns, data types, missing values, duplicates, and target distribution before model training.

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Random Forest Classifier
- Joblib
- Google Colab / Jupyter Notebook

## 🔄 Project Workflow

1. Import required libraries.
2. Download and load the dataset automatically.
3. Inspect data structure and quality.
4. Clean duplicate records and validate the target.
5. Perform exploratory data analysis.
6. Analyze churn patterns across customer characteristics.
7. Separate features and target variable.
8. Split data into training and testing sets.
9. Impute missing values and encode categorical features.
10. Train the Random Forest Classifier.
11. Evaluate model performance.
12. Visualize the confusion matrix and ROC curve.
13. Analyze feature importance.
14. Generate churn probabilities and risk categories.
15. Save the trained model and evaluation outputs.

## 🤖 Machine Learning Model

The project uses the **Random Forest Classifier**, an ensemble learning algorithm that combines multiple decision trees to make classification predictions.

The model uses:

- 300 decision trees
- A fixed random state for reproducibility
- Balanced class weights
- A training and testing split of 80% and 20%
- A preprocessing pipeline for missing values and categorical data

## 📈 Model Evaluation

The model is evaluated using the following metrics:

| Metric    | Description                                           |
| --------- | ----------------------------------------------------- |
| Accuracy  | Overall proportion of correct predictions             |
| Precision | How many predicted churn cases were actually churned  |
| Recall    | How many actual churn cases were correctly identified |
| F1-score  | Balance between precision and recall                  |
| ROC-AUC   | Ability to distinguish churned and retained customers |

The notebook also generates a confusion matrix and ROC curve.

**Note:** Actual model scores should be taken from the executed notebook. No performance score is assumed in advance.

## 📊 Feature Importance

The model calculates feature importance to identify which input features contribute most to its predictions.

These insights can help guide further investigation into customer behavior. Feature importance indicates predictive association, not proof of causation.

## 👥 Customer Churn Risk Prediction

The notebook generates:

- Actual churn labels for test records
- Predicted churn labels
- Predicted churn probabilities
- Low, medium, and high risk categories

The risk categories use illustrative probability thresholds and should be validated before real-world business use.

## 💼 Business Applications

- Identify customers who may be at risk of leaving.
- Support targeted customer retention campaigns.
- Investigate customer complaints and satisfaction patterns.
- Help prioritize customer engagement activities.
- Support data-driven marketing decisions.

## 🚀 How to Run the Project

### Option 1: Google Colab

1. Download `Ecommerce_Customer_Churn_Prediction.ipynb` from this repository.
2. Open [Google Colab](https://colab.research.google.com/).
3. Select **File → Upload notebook**.
4. Upload the downloaded notebook.
5. Run the notebook cells sequentially.
6. The dataset-download cell will retrieve the Excel file automatically.
7. Review the evaluation metrics, charts, and generated outputs.

An internet connection is required for the automatic dataset download.

### Option 2: Run Locally

Install the required packages:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn openpyxl joblib requests
```

Open the notebook in Jupyter Notebook or VS Code and execute the cells in order.

## 📁 Generated Outputs

The notebook saves the following files in the `outputs` directory:

- `random_forest_churn_model.joblib`
- `model_evaluation_results.csv`
- `feature_importance.csv`
- `customer_churn_predictions.csv`

These files are generated when the notebook runs successfully.

Avoid publishing customer-level predictions or sensitive data in a public repository.

## 🔮 Future Improvements

- Hyperparameter tuning with GridSearchCV or RandomizedSearchCV
- Cross-validation
- Decision-threshold optimization
- Comparison with Logistic Regression and Gradient Boosting
- Deployment using Streamlit or FastAPI
- Monitoring performance on future customer data

## ⚠️ Limitations

Model performance depends on data quality, representativeness, and class distribution. High accuracy alone does not guarantee effective churn detection. Recall, precision, and F1-score should also be considered.

Feature importance does not establish causation, and the model should be validated on future data before production deployment.


