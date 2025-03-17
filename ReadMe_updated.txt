Loan Eligibility Prediction Using Classification Models

Overview
This project aims to predict loan eligibility for applicants based on various financial and demographic attributes. The dataset includes key features like annual income, credit score, employment status, and loan amount. The objective is to classify applicants into "Approved" or "Rejected" categories using machine learning models.

Dataset
The dataset used in this project is loan_approval_dataset.csv, which contains:
- Numerical Features: Income, credit score, loan amount, etc.
- Categorical Features: Employment status, education level, etc.
- Target Variable: loan_status (Approved/Rejected)
- Project Workflow

1. Data Loading & Preprocessing
- Load dataset using Pandas.
- Handle missing values and data inconsistencies.
- Encode categorical variables using Label Encoding.
- Balance the dataset using SMOTE to address class imbalance.
- Split data into training (80%) and testing (20%) sets.

2. Exploratory Data Analysis (EDA)
- Generate visualizations such as:
- Bar plots & pie charts for categorical distributions.
- Histograms for credit score distribution.
- Scatter plots to analyze income vs. loan amount.
- Heatmap to explore feature correlations.

3. Model Training & Evaluation
Implemented three machine learning models:
a. Random Forest Classifier
- Used GridSearchCV to find optimal hyperparameters.
- Achieved high accuracy with best parameter tuning.
- Evaluated performance using classification report & ROC curve.
b. Gradient Boosting Classifier
- Applied boosting technique to improve classification.
- Conducted hyperparameter tuning using GridSearchCV.
- Compared results with Random Forest.
c. Logistic Regression
- Scaled features using StandardScaler.
- Trained and optimized model using GridSearchCV.
- Plotted ROC-AUC curve to measure performance.

4. Results & Model Comparison
- Compared accuracy scores across models.
- Visualized model performance with a bar chart.


Installation & Usage
Requirements
- Python 3.x
- Jupyter Notebook / Any Python IDE
- Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn, imbalanced-learn


