📞 Telecommunications Customer Classification using KNN

Skillset Employed: Python, Pandas, NumPy, Matplotlib, Seaborn, scikit-learn (sklearn), Data Analysis, Data Visualization, K-Nearest Neighbors (KNN)

📋 Project Description:

This project applies the K-Nearest Neighbors (KNN) algorithm to classify customers based on various attributes in the telecommunications sector. The model predicts customer categories using demographic and behavioral data, allowing businesses to better understand customer segments and tailor services accordingly.

Project Outcomes:
Exploratory Data Analysis (EDA):
Analyzed the dataset's structure and calculated summary statistics for features like region, tenure, income, and employment.
Visualized data distributions to understand feature ranges and identify potential outliers or trends.

Data Preprocessing:
Checked for missing values and duplicates to ensure data integrity.
Standardized features using StandardScaler for better performance of the KNN algorithm.
Split the dataset into training and testing sets to evaluate model performance effectively.

Modeling with K-Nearest Neighbors:
Built a KNN classifier to predict customer categories.
Experimented with different values of k to find the optimal k-value for the best performance.
Evaluated the model using train and test accuracies, with k=4 selected as the optimal value due to minimal variance between training and testing accuracy.

Model Evaluation:
Evaluated the KNN model using key metrics:
Train Set Accuracy: 82.4% for k=4
Test Set Accuracy: 71.0% for k=4
Iterated over multiple k values to observe accuracy trends and selected the most stable model.

📊 Visualizations:

1. Histogram: Income Distribution 💰
A histogram showcasing the distribution of customer income.
Provides insights into the income levels of the customers, helping to understand their purchasing power and financial demographics.
2. Accuracy Evaluation for Different K Values 📈
Iteratively tested different k values and plotted their accuracy.
Identified k=4 as the optimal value due to its balanced accuracy between training and testing sets.


🛠️ Tools & Libraries Used:

Python: Programming language for data analysis and modeling.
Pandas & NumPy: Data manipulation and numerical operations.
Matplotlib & Seaborn: Visualization of data distributions and relationships.
scikit-learn (sklearn): For building and evaluating the KNN classifier.

📁 Dataset:

Dataset Name: TeleCust.csv
Description: Contains customer data, including demographic details like region, tenure, age, income, and other relevant attributes.
Columns: region, tenure, age, marital, address, income, ed, employ, retire, gender, reside, custcat.

💡 Key Takeaways:

1. KNN is a powerful but simple algorithm for classification tasks, especially when dealing with demographic and behavioral data.

2. Selecting the optimal k-value is crucial for balancing model accuracy between training and testing sets.

3. Data normalization is important for algorithms like KNN that rely on distances between data points.
