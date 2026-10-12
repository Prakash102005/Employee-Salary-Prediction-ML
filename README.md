# 💼 Employee Salary Prediction Using Machine Learning
### Supervised Regression | Python + Scikit-Learn

> Regression models predicting employee salary from age, gender, education, job title and experience. The **Random Forest** performed best: **R² = 0.90, RMSE ≈ $15.6K** on a held-out test set.

---

## 🎯 Objective
**👉 Predict an employee's salary from demographic, educational and professional attributes.**

This is a **supervised regression problem**, where the target variable is `Salary`.

---

## 📈 Results
Evaluated on a held-out 20% test set (about 75 records):

| Model | R² Score | RMSE |
|---|---|---|
| Linear Regression | unstable* | unstable* |
| Decision Tree Regressor | 0.8562 | 18,565 |
| **Random Forest Regressor** | **0.8991** | **15,553** |
| Gradient Boosting Regressor | 0.8818 | 16,836 |

\* Plain Linear Regression was numerically unstable on 170+ one-hot columns with only about 300 training rows, so its score is not meaningful. Regularised regression (Ridge) is listed under Future Improvements.

- Tree-based ensembles clearly outperformed a single Decision Tree
- Random Forest's RMSE of about **$15.6K is roughly 15% of the average salary** ($100.6K)

<!-- Optional: add a chart after saving it to an images/ folder
![Salary Distribution](images/salary_distribution.png)
-->

---

## 📂 Dataset
- **Source:** Salary Data (CSV)
<!-- Add the dataset link here, e.g. Kaggle: [Salary Data](URL) -->
- **Records:** 375 rows, 373 after dropping rows with missing values
- **Target Variable:** `Salary` (mean ≈ $100.6K, range $350 – $250K)

| Feature | Description |
|---|---|
| Age | Employee age (23–53) |
| Gender | Male / Female |
| Education Level | Bachelor's, Master's, PhD |
| Job Title | Employee designation (170+ unique titles) |
| Years of Experience | 0–25 years |
| Salary | Target variable |

---

## ⚙️ Methodology

### 🔹 1. Data Exploration
Checked structure, data types, missing values and summary statistics; plotted the salary distribution (histogram + KDE).

### 🔹 2. Data Preprocessing
- Dropped rows with missing values (2 rows)
- Mapped **Gender** to numeric (Male = 1, Female = 0)
- **One-hot encoded** Education Level and Job Title (`drop_first=True`)
- 80/20 train-test split (`random_state=42`)

### 🔹 3. Model Development
Trained and compared four regressors: **Linear Regression** (baseline), **Decision Tree**, **Random Forest** and **Gradient Boosting**.

### 🔹 4. Model Evaluation
Models compared using **R² Score** and **RMSE** on unseen test data.

---

## ⚠️ Limitations
- **Small dataset** (373 rows): the test set has only about 75 records, so scores may vary with a different split
- **Many job titles with few examples each**, so models may partly memorise title → salary
- Default hyperparameters and a single train-test split (no tuning or cross-validation yet)

---

## 🗂 Project Structure
```
├── Employee Salary Prediction - ML Project.ipynb
├── Salary Data.csv
├── requirements.txt
└── README.md
```

## ▶️ How to Run
```bash
git clone https://github.com/Prakash102005/Employee-Salary-Prediction-ML.git
cd Employee-Salary-Prediction-ML
pip install -r requirements.txt
jupyter notebook "Employee Salary Prediction - ML Project.ipynb"
```
Update the CSV path in the notebook so it points to `Salary Data.csv` in the project folder.

---

## 🛠 Tools & Technologies
**Python** (Pandas, NumPy, Matplotlib, Seaborn) · **Scikit-learn** · Jupyter Notebook

---

## 👤 Author
**Saiprakash Yamsani** | [GitHub](https://github.com/Prakash102005) | [LinkedIn](https://www.linkedin.com/in/)
