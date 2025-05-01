# 🚗 CO₂ Emissions Prediction Using Simple Linear Regression

## 🧠 Skillset & Technologies Used

**Languages & Libraries**:  
Python, Pandas, NumPy, Matplotlib, PyPlot, scikit-learn (sklearn)  

**Skills**:  
Exploratory Data Analysis (EDA), Data Cleaning, Data Visualization, Linear Regression Modeling, Model Evaluation, Feature Engineering

**System & Data Ecosystem**:  
- Data Source: Vehicle specifications dataset (`FuelConsumptionCo2.csv`)  
- Data Pipeline: CSV → Pandas DataFrame → EDA → Modeling using scikit-learn → Evaluation & Visualization  
- Visualization Layer: Matplotlib / PyPlot for trends and correlations  
- Modeling Layer: Simple Linear Regression Model  
- Deployment Target: Ideal for integration into vehicle emission analytics platforms

---

## 📊 Business Context

Government agencies and automobile manufacturers need tools to **monitor and reduce CO₂ emissions** to meet climate and regulatory goals. By analyzing how vehicle characteristics (e.g., engine size, fuel consumption) relate to emissions, organizations can **optimize engine designs** and promote fuel-efficient vehicles.

---

## 📁 Dataset Overview

**Dataset**: `FuelConsumptionCo2.csv`  
**Description**: Contains data on fuel consumption and CO₂ emissions for multiple vehicles.  

**Key Dimensions (Descriptive)**:
- `MAKE`: Vehicle brand
- `MODEL`: Specific vehicle model
- `VEHICLECLASS`: Type of vehicle (e.g., SUV, Sedan)
- `FUELTYPE`: Type of fuel used
- `TRANSMISSION`: Transmission type

**Key Metrics (Quantitative)**:
- `ENGINESIZE`: Engine capacity (liters)
- `CYLINDERS`: Number of cylinders
- `FUELCONSUMPTION_COMB`: Combined fuel consumption (L/100km)
- `FUELCONSUMPTION_COMB_MPG`: Miles per gallon
- `CO2EMISSIONS`: CO₂ emissions in grams/km

---

## 📊 Exploratory Data Analysis (EDA)

- Checked for **missing/null values** and ensured data cleanliness.
- Performed **summary statistics** on numerical features.
- Identified potential **correlations** between engine size, fuel consumption, and emissions.

---

## 📈 Visual Insights

1. **Engine Size vs CO₂ Emissions**  
   - Strong positive linear relationship.
   - Larger engines tend to emit more CO₂.

2. **Fuel Consumption (Combined) vs CO₂ Emissions**  
   - Vehicles with higher fuel consumption contribute more to emissions.

3. **Cylinders vs CO₂ Emissions**  
   - Higher cylinder count generally leads to increased emissions.

4. **Distribution of Training Data**  
   - Regression line shows a clear linear trend, supporting model validity.

---

## 🤖 Machine Learning Model

### Model Used:  
**Simple Linear Regression** with `Engine Size` as the independent variable and `CO2 Emissions` as the dependent variable.

### Data Split:  
- Training: 80%  
- Testing: 20%

### Evaluation Metrics:
- **Mean Absolute Error (MAE)**: 22.63
- **Mean Squared Error (MSE)**: 854.93
- **R² Score**: 0.79 (Good fit)

---

## 💡 Key Insights

- **Engine Size is a reliable predictor** of CO₂ emissions.
- Fuel-efficient designs (lower engine size and consumption) **substantially reduce emissions**.
- Visualization helps stakeholders **clearly see the impact** of vehicle design on environmental footprint.

---

## ✅ Recommendations

- **Policy Makers**: Enforce stricter emission caps on high-engine vehicles.
- **Auto Manufacturers**: Invest in smaller or hybrid engines to meet sustainability goals.
- **Consumers**: Encourage purchasing of vehicles with lower fuel consumption and smaller engines.

---

## 📦 Future Improvements

- Integrate additional features like `Vehicle Weight`, `Drive Type` for better accuracy.
- Try **Multivariable Regression** to incorporate multiple predictors.
- Deploy model using **Flask API** or **Streamlit dashboard** for real-time use.

---

## 📬 Contact

For queries or suggestions, please reach out at [ywuyyuru7@gmail.com]

---



