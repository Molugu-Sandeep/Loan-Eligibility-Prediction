# Loan-Eligibility-Prediction
This code appears to be the beginning of a loan eligibility prediction project using a classification model.
1. Libraries: It starts by importing essential libraries for data manipulation (pandas, numpy), machine learning (sklearn), and visualization (matplotlib, seaborn).
2. Data Loading: It loads a dataset named "loan_approval_dataset.csv" using pandas.
3. Data Exploration: It performs initial data exploration:
- Viewing the top few rows of the dataset using data.head()
- Checking for missing values (NaN) using data.isna().sum()
- Inspecting data types and overall information using data.info()
4. Data Visualization: It creates visualizations to understand the data:
- A countplot of 'loan_status' to see the distribution of loan approvals and rejections.
- Pie charts for 'education' and 'self_employed' to illustrate the proportion of applicants with different educational backgrounds and employment statuses.
- A histogram of 'credit_score' to analyze the distribution of applicant credit scores.

Feature Engineering
This section focuses on preparing the data for model training by addressing issues like:

Mapping Loan Status: The 'loan_status' column is transformed into numerical values (1 for 'Approved', 0 for 'Rejected') to make it suitable for machine learning algorithms.
One-Hot Encoding: Categorical features like ' education', ' self_employed', etc., are converted into numerical representations using one-hot encoding. This process creates new binary columns for each unique category, allowing models to interpret them effectively.
Model Building
This part involves training and evaluating different machine learning models to predict loan eligibility:

Random Forest Model
A Random Forest model is initialized with 100 decision trees for better accuracy and robustness.
The model is trained using the training data (X_train, y_train).
Predictions are made on the testing data (X_test).
The model's accuracy and performance metrics like precision, recall, and F1-score are evaluated using the predicted outcomes (y_pred_rf) against the actual outcomes (y_test).
Gradient Boosting Classifier
A Gradient Boosting model is initialized with 100 estimators, aiming to achieve high accuracy.
The model is trained using the training dataset.
Predictions are generated for the testing data.
The model's accuracy and other performance metrics are calculated using the actual and predicted outcomes.
Model Evaluation
This segment evaluates the performance of the trained models:

ROC Curve and AUC
ROC (Receiver Operating Characteristic) curves are plotted for both the Random Forest and Gradient Boosting models.
The Area Under the Curve (AUC) is calculated, indicating the model's ability to distinguish between loan approval and rejection. A higher AUC suggests better model performance.
Model Accuracy Comparison
A bar chart is used to visually compare the accuracy of both the Random Forest and Gradient Boosting models. This allows for a quick assessment of which model performs better in terms of overall prediction accuracy
