# 💼 Employee Salary Prediction Using Machine Learning

> A Machine Learning project that predicts employee salaries based on demographic, educational, and professional attributes using various regression algorithms.

---

## 🚀 Project Overview

This project focuses on predicting employee salaries based on various factors such as **age**, **gender**, **education level**, **job title**, and **years of experience**. Multiple machine learning regression algorithms are trained and evaluated to identify the model that provides the most accurate salary predictions.

The project demonstrates the complete machine learning workflow, including data preprocessing, exploratory data analysis, feature engineering, model training, and performance evaluation.

---

## 🎯 Problem Statement

Determining an employee's salary based on their qualifications and experience can be challenging. Traditional methods often rely on fixed salary structures and manual assessments.

The goal of this project is to build a predictive model capable of accurately estimating salaries using employee-related attributes.

---

## 📌 Objectives

The primary objectives of this project are:

- 📊 Analyze employee salary data
- 🧹 Perform data cleaning and preprocessing
- 🔍 Explore relationships between features and salary
- 🔠 Transform categorical data into machine-readable format
- 🤖 Train multiple regression models
- 📉 Compare model performances
- ✅ Select the best-performing model for salary prediction

---

## 📂 Dataset Features

The dataset contains the following attributes:

| Feature               | Description                         |
|-----------------------|-------------------------------------|
| Age                   | Employee age                        |
| Gender                | Male / Female                       |
| Education Level       | Bachelor's, Master's, PhD, etc.     |
| Job Title             | Employee designation                |
| Years of Experience   | Total years of work experience      |
| Salary                | Target variable (Employee Salary)   |

---

## 🛠️ Technologies Used

### Languages & Libraries

| Tool            | Purpose                        |
|-----------------|-------------------------------|
| Python          | Core programming language     |
| Pandas          | Data manipulation             |
| NumPy           | Numerical computations        |
| Matplotlib      | Data visualization            |
| Seaborn         | Statistical plots             |
| Scikit-Learn    | Machine learning models       |
| Jupyter Notebook| Interactive development       |

### Development Environment
- ☁️ **Google Colab**

---

## 📊 Project Workflow

### 1. 📥 Import Libraries
Required libraries for data manipulation, visualization, and machine learning are imported.

### 2. 📁 Load Dataset
The employee salary dataset is loaded using Pandas.

### 3. 🔎 Data Exploration
- View dataset structure
- Check data types
- Analyze missing values
- Generate statistical summaries

### 4. 📉 Data Visualization
Salary distribution is visualized using histogram plots to understand data spread.

### 5. ⚙️ Data Preprocessing
- Remove missing values
- Convert **Gender** into numerical format
- Apply **One-Hot Encoding** to:
  - Education Level
  - Job Title

### 6. 🎯 Feature Selection
Features (`X`) and target variable (`y`) are separated.

### 7. ✂️ Train-Test Split
Dataset is divided into training and testing sets.

### 8. 🤖 Model Training
The following regression models are trained:
- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor

### 9. 📈 Model Evaluation
Models are evaluated using:
- **R² Score**
- **Root Mean Squared Error (RMSE)**

---

## 🤖 Machine Learning Models

### 🔹 Linear Regression
A baseline regression model that assumes a linear relationship between features and salary.

### 🔹 Decision Tree Regressor
A tree-based model that captures non-linear relationships.

### 🔹 Random Forest Regressor
An ensemble learning technique that combines multiple decision trees for better accuracy.

### 🔹 Gradient Boosting Regressor
A boosting algorithm that builds models sequentially to minimize prediction errors.

---

## 📈 Evaluation Metrics

### R² Score
Measures how well the model explains the variance in salary data.

### RMSE (Root Mean Squared Error)
Measures the average prediction error in salary estimation.

---

## 💡 Key Learnings

- Handling missing data and encoding categorical variables for ML models
- Comparing multiple regression algorithms using R² and RMSE metrics
- Understanding the impact of features like job title and education on salary prediction

---

## 👨‍💻 Author

**Saiprakash Yamsani**

*Machine Learning Project – Employee Salary Prediction using Python and Scikit-Learn.*
