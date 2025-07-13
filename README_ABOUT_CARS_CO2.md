# 📊 CO2 Emission Prediction - Linear Regression Project

This project aims to **predict CO2 emissions** from vehicles using features such as fuel consumption and engine characteristics. The model is trained using **Linear Regression**, and two different scaling techniques are compared to evaluate model performance.

---

## 🔍 Project Objective

To predict the amount of **CO2 emissions** using the following features:

- `FUELCONSUMPTION_CITY`: Fuel consumption in the city  
- `FUELCONSUMPTION_HWY`: Fuel consumption on the highway  
- `CYLINDERS`: Number of engine cylinders

---

## 🧪 Project Steps

### 1. Data Cleaning & Preprocessing  
The dataset was loaded and checked for missing or invalid values. Then the relevant features were selected into a new DataFrame (`cdf`) for further analysis.

### 2. Exploratory Data Analysis (EDA)  
Three scatter plots were created to visualize the relationship between each feature and CO2 emissions:

- Fuel consumption in the city vs. CO2  
- Number of cylinders vs. CO2  
- Fuel consumption on the highway vs. CO2  

🎯 These plots help to visually evaluate if linear regression is a suitable model.

### 3. Feature Scaling  
To improve model accuracy, data was normalized using two different scalers:

- `StandardScaler`  
- `MinMaxScaler`  

Both scaled datasets were used to train separate regression models.

### 4. Model Training & Evaluation  
Linear Regression was applied to both scaled datasets. The model performance was evaluated using the following metrics:

- **MAE** (Mean Absolute Error)  
- **MSE** (Mean Squared Error)  
- **R² Score** (Coefficient of Determination)

---

## 📈 Results

Scatter plots were created to compare actual CO2 emissions versus predicted values for each scaling method. This helped evaluate which scaler produced more accurate results.

---

## 🛠 How to Run the Project

1. **Install dependencies:**

```bash
pip install pandas numpy matplotlib scikit-learn
