#Credit Card Fraud Detection Using Machine Learning

##Skillset & Technologies Used

**Languages & Libraries**:  
Python, Pandas, NumPy, Matplotlib, Seaborn, scikit-learn, imbalanced-learn (SMOTE), joblib  

**Skills**:  
Exploratory Data Analysis (EDA), Data Cleaning, Feature Engineering, Model Building & Evaluation, Imbalanced Data Handling, Model Deployment

**System & Data Ecosystem**:  
- **Data Source**: Anonymized credit card transactions dataset  
- **Data Pipeline**: CSV → DataFrame (Pandas) → Preprocessing → Model Training → Evaluation → Serialization using `joblib`  
- **Modeling Layer**: Multiple classifiers (Logistic Regression, Decision Tree, Random Forest)  
- **Monitoring Layer**: Evaluation metrics, confusion matrix, classification reports  
- **Imbalance Handling**: SMOTE for oversampling minority class  
- **Deployment Readiness**: Models saved for downstream fraud detection API or dashboard use

---

##Business Context

Fraudulent transactions cause billions in annual losses to financial institutions. Timely and accurate fraud detection is vital for:
- Protecting customer trust
- Reducing chargeback costs
- Ensuring regulatory compliance

This project aims to build an **automated detection system** that flags fraudulent activities using real transaction data.

---

##Dataset Overview

**Dataset**: `creditcardtransactiondata.csv`  
**Description**: Contains anonymized credit card transactions labeled as fraud or normal.  

### Dimensions (Categorical Descriptors):
- `Class`: Indicates transaction type — 0 (Normal), 1 (Fraud)

### Metrics (Quantitative Measures):
- `Time`: Seconds elapsed between this transaction and the first transaction in the dataset
- `Amount`: Transaction amount
- `V1-V28`: Anonymized features derived from PCA transformation of original features

---

##Exploratory Data Analysis (EDA)

- Validated the dataset for missing values and duplicates
- Identified **strong class imbalance** (~0.17% of transactions are fraud)
- Standardized `Time` and `Amount` using `StandardScaler` for model compatibility
- Used **correlation matrix (heatmap)** to study inter-feature relationships

---

##Data Preprocessing

- **Class Balancing**:  
  - **Undersampling**: Balanced the dataset by reducing normal transactions  
  - **SMOTE**: Applied Synthetic Minority Oversampling to increase fraudulent examples during training

- **Feature Scaling**:  
  - Applied `StandardScaler` to normalize `Time` and `Amount`

- **Label Encoding**:  
  - No transformation required as target `Class` is binary

---

##Visualizations & Key Insights

1. **Fraud vs Normal Transaction Distribution**  
   - Visualized severe class imbalance, emphasizing the challenge of model training

2. **Correlation Heatmap**  
   - Revealed potential multicollinearity among features  
   - Helped reduce model complexity by deprioritizing low-impact features

3. **Confusion Matrix (Per Model)**  
   - Illustrated true positives, false negatives, etc., for Logistic Regression, Decision Tree, and Random Forest

---

##Models & Evaluation

### Models Trained:
- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier ✅ (Best Performer)

### Evaluation Metrics:
- **Accuracy Score**
- **Precision, Recall, F1-Score** (From Classification Report)
- **ROC-AUC Score**
- **Confusion Matrix** (TP, TN, FP, FN breakdown)

### Final Model Performance (Random Forest):
- **High Precision & Recall** on SMOTE-balanced data
- Excellent generalization with reduced false negatives

---

##Business Insights

- **Transaction Amount & Time play a significant role** in identifying potential fraud.
- **Random Forest models are highly effective** in flagging fraudulent transactions without heavy cost of false positives.
- **Balancing datasets (via SMOTE)** drastically improves recall — critical in fraud detection.
- Fraud detection must prioritize **recall over precision** to avoid missing actual fraud cases.

---

##Strategic Recommendations

- **Implement Random Forest as core fraud detection engine** with periodic retraining using fresh transaction data.
- Integrate model with **real-time fraud alert systems** to trigger customer notifications or transaction holds.
- Regularly **monitor drift in features** (e.g., distribution of Amount or Time) using dashboards.
- Consider **unsupervised anomaly detection models** for identifying emerging fraud patterns not present in labeled data.

---

##Future Enhancements

- Incorporate **real-time streaming data** pipelines (e.g., Apache Kafka + Spark)
- Evaluate **deep learning models** like Autoencoders for anomaly detection
- Deploy the model as an API using **Flask** or **FastAPI**
- Build a monitoring dashboard using **Power BI** or **Streamlit**

---

##Contact

For feedback or collaboration: [yaswanth.wuyyuru@hotmail.com]
