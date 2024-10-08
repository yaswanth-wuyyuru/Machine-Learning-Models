🚗 Simple Linear Regression for Fuel Consumption & CO₂ Emissions Prediction

Skillset Employed: Python, Pandas, NumPy, Matplotlib, PyPlot, scikit-learn (sklearn), Data Analysis, Data Visualization, Machine Learning

📋 Project Description:

This project utilizes Simple Linear Regression to analyze the relationship between vehicle Engine Size and CO₂ Emissions. Using a dataset of vehicle specifications, we explore how changes in engine size and other vehicle features influence CO₂ emissions. The analysis leverages scikit-learn for building the regression model and Matplotlib for visualizing relationships.

Project Outcomes:
Exploratory Data Analysis (EDA):
Analyzed the dataset's structure and calculated summary statistics for features like engine size, cylinders, and fuel consumption.
Ensured data quality through checks for null values and performed data cleaning where necessary.
Data Visualization:
Visualized relationships between different vehicle features and CO₂ Emissions using scatter plots:
Relationship between Engine Size and CO₂ Emissions.
Impact of Fuel Consumption Combination on CO₂ Emissions.
Relationship between Cylinders and CO₂ Emissions.
Histograms were used to display the distribution of key features.
Data Modeling:
Built a Simple Linear Regression Model to predict CO₂ Emissions based on Engine Size.
Used 80% of the dataset for training and 20% for testing, ensuring a robust evaluation of model performance.
Model Evaluation:
Evaluated model performance using key metrics:
Mean Absolute Error (MAE): 22.63
Mean Squared Error (MSE): 854.93
R² Score: 0.79
The high R² score indicates that the model effectively captures the relationship between Engine Size and CO₂ Emissions.
📊 Visualizations:

1. Scatter Plot: Engine Size vs. CO₂ Emissions 🔵
This plot illustrates the positive linear relationship between Engine Size and CO₂ Emissions.
As the Engine Size increases, the CO₂ Emissions also tend to increase.
2. Scatter Plot: Fuel Consumption Combination vs. CO₂ Emissions 🔴
Shows the impact of combined fuel consumption on CO₂ Emissions.
Higher fuel consumption generally leads to higher CO₂ emissions.
3. Scatter Plot: Cylinders vs. CO₂ Emissions 🟢
Explores how the number of cylinders affects CO₂ Emissions.
Vehicles with more cylinders tend to produce higher CO₂ Emissions.
4. Train Data Distribution 🟣
Visualizes the distribution of training data points for Engine Size and CO₂ Emissions.
The linear trend is highlighted with a regression line.
🛠️ Tools & Libraries Used:

Python: Programming language for data analysis and modeling.
Pandas & NumPy: Data manipulation and numerical operations.
Matplotlib & PyPlot: Visualization of data relationships.
scikit-learn (sklearn): For building and evaluating the Linear Regression model.
📁 Dataset:

Dataset Name: FuelConsumptionCo2.csv

Description: Contains data on vehicle specifications, fuel consumption, and CO₂ emissions.

Columns: MODELYEAR, MAKE, MODEL, VEHICLECLASS, ENGINESIZE, CYLINDERS, TRANSMISSION, FUELTYPE, FUELCONSUMPTION_CITY, FUELCONSUMPTION_HWY, FUELCONSUMPTION_COMB, FUELCONSUMPTION_COMB_MPG, CO2EMISSIONS.

💡 Key Takeaways:

The linear regression model provides a strong understanding of how Engine Size influences CO₂ Emissions.
Through visualization, stakeholders can make data-driven decisions and optimize vehicle designs to reduce emissions.
