
#  Student Exam Score Prediction – Linear & Polynomial Regression

##  Project Overview

This project is part of my internship task where I explored **Regression Models** to predict students' exam scores.
The goal was to understand how factors like **hours studied, attendance, sleep, and previous scores** affect exam performance, and to build models that can make predictions.

I implemented:

* ✅ **Linear Regression (Single Feature)** – using only study hours
* ✅ **Polynomial Regression** – to capture non-linear patterns
* ✅ **Multiple Linear Regression** – using multiple factors like attendance, sleep, etc.

The project also includes **data cleaning, visualization, model evaluation, and performance comparison**.

---

##  Dataset

The dataset used: **Student Performance Factors** (from Kaggle).
It contains features such as:

* `Hours_Studied` – number of hours studied
* `Attendance` – percentage of classes attended
* `Sleep_Hours` – average daily sleep
* `Previous_Scores` – past exam scores
* `Exam_Score` – target variable to predict

---

## 🛠️ Tools & Libraries

* **Python**
* **Pandas** → data handling
* **Matplotlib** → visualization
* **Scikit-learn** → regression models & metrics
* **NumPy** → mathematical operations

---

##  Steps Performed

### 1. **Data Cleaning**

* Dropped rows with missing values in key columns (`Exam_Score`, `Hours_Studied`).
* Filled remaining missing numeric values with median.
* Removed duplicate rows.

### 2. **Exploratory Data Analysis (EDA)**

* Scatter plots between **study hours** and **exam score**.
* Visualization of actual vs predicted scores.
* Feature importance analysis using regression coefficients.

### 3. **Model Training & Evaluation**

* **Single Variable Linear Regression** → trained with only `Hours_Studied`.
* **Polynomial Regression (degree=2)** → added squared study hours for better curve fitting.
* **Multiple Linear Regression** → used multiple features (`Hours_Studied`, `Attendance`, `Sleep_Hours`, `Previous_Scores`).

Evaluation Metrics used:

* MAE (Mean Absolute Error)
* MSE (Mean Squared Error)
* R² Score

### 4. **Visualization**

* **Linear vs Polynomial Fit** plots
* **Actual vs Predicted** scatter plots
* **Feature Importance (bar chart of coefficients)**

---

##  Results & Learnings

* **Linear Regression (1 feature):** Simple but limited in capturing complex relationships.
* **Polynomial Regression:** Better performance when the relationship is curved, not straight.
* **Multiple Linear Regression:** Most reliable, since exam score depends on many factors, not just study hours.

 **Key Insight:** More features = better prediction, but also risk of overfitting. Polynomial regression can improve performance if data is non-linear.

---

##  How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/Student_Score_Prediction.git
   ```
2. Install required libraries:

   ```bash
   pip install pandas matplotlib scikit-learn numpy
   ```
3. Run the Jupyter Notebook or Python script.

---

##  Future Improvements

* Try advanced models (Ridge, Lasso, Random Forest).
* Hyperparameter tuning for polynomial degree.
* Add more visualizations for deeper analysis.

---

## Acknowledgement

Dataset: [Kaggle – Student Performance Factors](https://www.kaggle.com/)

---

