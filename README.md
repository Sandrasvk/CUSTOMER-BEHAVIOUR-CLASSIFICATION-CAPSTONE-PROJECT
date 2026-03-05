# Customer Behaviour Classification & Model Deployment

## 📌 Project Overview
This project aims to predict customer purchasing decisions by analyzing demographic and financial data from a client base of 400 individuals. It includes a complete data science workflow from data cleaning to real-time model deployment via a desktop GUI.

## 📊 Dataset Detail
The analysis is based on the Customer_Behaviour.csv dataset, which includes the following features:
* *Gender*: Categorical feature (Encoded: Female = 1, Male = 0).
* *Age*: Numerical age of the customer.
* *EstimatedSalary*: Annual estimated salary.
* *Purchased (Target)*: Binary classification (1 if the customer purchased the product, 0 otherwise).

## 🛠️ Implementation Steps
### 1. Data Cleaning & Preprocessing
* *Null Value Check*: Verified that the dataset contains no missing values.
* *Feature Selection*: The User ID column was removed as it does not contribute to the prediction model.
* *Categorical Encoding*: Converted the Gender column into binary numerical values using a custom function.

### 2. Exploratory Data Analysis (EDA)
* Used *Seaborn Heatmaps* to visualize and analyze the correlation between Age, Salary, and Purchase behavior.
* I have used pairplots, countplots etc for the data visualization

### 3. Feature Scaling (Standard Scaler used)
* Splitted input and target variables
* I have used Standard Scaler for the feature scaling
* * Train test Split : The model are selected for train test split. 80% are used for training and 20% for testing
* I have used various ML algorithms like Logistic Regression, Random Forest, Support Vector Machine
* Used cross val scores of all models into a dataframe

### 4. Model Deployment (GUI)
The project features a functional desktop application created with the *Tkinter* library to allow for interactive predictions:
* *Input Fields: Users can enter a customer's **Age* and *Salary*.
* Used combobox for gender
* *Functionality*: A "Get Prediction" button triggers the model to output the result directly in the interface.

## 🧰 Libraries & Tools
* *Pandas & NumPy*: Data manipulation and numerical operations.
* *Matplotlib & Seaborn*: Statistical data visualization.
* *Tkinter*: Graphical User Interface (GUI) development.
* *Scikit-learn*: Machine learning model implementation.

## 🚀 Execution
To run the project, ensure you have the Customer_Behaviour.csv file in the same directory as the notebook and execute the cells to launch the Tkinter interface.
I have done this in jupyter Notebook
