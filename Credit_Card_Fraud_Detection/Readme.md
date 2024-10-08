💳 Credit Card Fraud Detection using Machine Learning

Skillset Employed: Python, Pandas, NumPy, Matplotlib, Seaborn, scikit-learn (sklearn), imbalanced-learn (SMOTE), Data Analysis, Data Visualization, Model Evaluation, Machine Learning

📋 Project Description:

This project employs Machine Learning techniques to detect fraudulent credit card transactions. It leverages a variety of classifiers, including Logistic Regression, Decision Trees, and Random Forest, to distinguish between normal and fraudulent transactions. With techniques like SMOTE (Synthetic Minority Over-sampling Technique), the project addresses the challenges of class imbalance, enhancing model performance on minority class detection.

Project Outcomes:
Exploratory Data Analysis (EDA):
Analyzed the dataset and calculated statistical metrics for features such as transaction time, amount, and anonymized V1-V28 features.
Visualized the distribution of normal vs. fraudulent transactions, highlighting the class imbalance.
Data Preprocessing:
Checked for missing values and handled duplicates, ensuring data quality.
Standardized features like Time and Amount using StandardScaler to ensure uniformity.
Addressed class imbalance using undersampling and SMOTE, ensuring balanced datasets for better model training.
Data Visualization:
Generated a heatmap to visualize correlations among features, helping identify relationships and feature redundancies.
Created plots to showcase the distribution and relationships between features.
Modeling & Evaluation:
Trained three models: Logistic Regression, Decision Tree, and Random Forest on the preprocessed data.
Evaluated models using key metrics:
Accuracy Score
ROC AUC Score
Confusion Matrix
Classification Report (Precision, Recall, F1-score)
The Random Forest classifier demonstrated high performance, with near-perfect precision and recall on balanced datasets.
Handling Imbalanced Data:
Initially, used undersampling to match normal transactions to the number of fraudulent transactions.
Applied SMOTE for generating synthetic samples, ensuring that the training data is balanced and the model generalizes well to both classes.
📊 Visualizations:

1. Distribution of Fraud vs. Normal Transactions 📊

A bar plot visualizing the count of normal and fraudulent transactions, highlighting the imbalance in the dataset.
Provides insights into the challenge of fraud detection due to the relatively small number of fraudulent transactions.

2. Heatmap: Correlation Matrix 🔍

A heatmap illustrating correlations between anonymized features.
Helps identify potentially redundant features and understand feature relationships.

3. Confusion Matrix for Classifiers 📈

Provides insights into true positives, true negatives, false positives, and false negatives for each model.
Essential for understanding the model's performance on detecting fraudulent transactions.
🛠️ Tools & Libraries Used:

Python: Programming language for data analysis and modeling.
Pandas & NumPy: Data manipulation and numerical operations.
Matplotlib & Seaborn: Visualization of data relationships.
scikit-learn (sklearn): For building and evaluating classifiers.
imbalanced-learn (SMOTE): To handle class imbalance and improve model training.
joblib: For saving and loading trained models.
📁 Dataset:

Dataset Name: creditcardtransactiondata.csv
Description: Contains anonymized data on credit card transactions, including Time, Amount, anonymized V1-V28 features, and Class (0: Normal, 1: Fraud).
Columns: Time, V1, V2, ..., V28, Amount, Class.

💡 Key Takeaways:

Addressing class imbalance is critical for effective fraud detection. 

Techniques like SMOTE ensure balanced training.

The Random Forest classifier proved to be the most effective in detecting fraudulent transactions with high precision and recall.

Visualizations play a crucial role in understanding data distributions and feature relationships, guiding model selection and improvement.
