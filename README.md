# OIBSIP_Data-Science_taskno.5
# Sales Prediction Using Python

## 📈 Project Overview

This project was completed as part of the **Oasis Infobyte Data Science Internship (Task 5)**.

The objective of this project is to build a Machine Learning model that predicts product sales based on advertising expenditures across different marketing platforms such as TV, Radio, and Newspaper.

Businesses invest significant amounts in advertising, and predicting future sales helps organizations optimize their marketing budgets and make data-driven decisions.

This project demonstrates the complete Machine Learning workflow including data exploration, preprocessing, model training, evaluation, and sales prediction.

---

## 📊 Dataset Information

Dataset: **Advertising Dataset**

### Dataset Source

https://www.kaggle.com/datasets/bumba5341/advertisingcsv

The dataset contains advertising expenditure data across various media platforms and corresponding sales figures.

---

## 📋 Dataset Features

| Feature   | Description                           |
| --------- | ------------------------------------- |
| TV        | Advertising budget spent on TV        |
| Radio     | Advertising budget spent on Radio     |
| Newspaper | Advertising budget spent on Newspaper |
| Sales     | Product Sales (Target Variable)       |

### Example

| TV    | Radio | Newspaper | Sales |
| ----- | ----- | --------- | ----- |
| 230.1 | 37.8  | 69.2      | 22.1  |

This means:

* TV Advertisement Budget = 230.1
* Radio Advertisement Budget = 37.8
* Newspaper Advertisement Budget = 69.2
* Sales Generated = 22.1

---

## 🎯 Project Objectives

* Analyze advertising and sales data.
* Explore relationships between marketing expenditure and sales.
* Build a Machine Learning regression model.
* Predict future sales based on advertisement spending.
* Evaluate model performance using regression metrics.

---

## 🛠 Technologies Used

* Python
* Pandas
* Scikit-Learn
* Jupyter Notebook
* Machine Learning

---

## 🤖 Machine Learning Algorithm

### Linear Regression

Linear Regression is a supervised Machine Learning algorithm used to predict continuous numerical values.

In this project, it learns the relationship between:

* TV Advertising Budget
* Radio Advertising Budget
* Newspaper Advertising Budget

and

* Sales

### Why Linear Regression?

✅ Simple and Effective

✅ Easy to Interpret

✅ Works Well for Numerical Prediction

✅ Suitable for Sales Forecasting Problems

---

## 📂 Project Workflow

### Step 1: Import Required Libraries

Libraries Used:

* Pandas
* train_test_split
* LinearRegression
* r2_score
* mean_absolute_error

---

### Step 2: Load Dataset

The dataset is loaded into a Pandas DataFrame for analysis and preprocessing.

---

### Step 3: Data Exploration

Performed operations:

* Display first five rows
* Check dataset shape
* Check dataset information
* Identify missing values

---

### Step 4: Data Preprocessing

If present, the unnecessary index column (`Unnamed: 0`) is removed.

---

### Step 5: Define Features and Target

#### Features (X)

* TV
* Radio
* Newspaper

#### Target (y)

* Sales

---

### Step 6: Train-Test Split

Dataset is divided into:

* Training Data: 80%
* Testing Data: 20%

Random State:

42

---

### Step 7: Train Machine Learning Model

A Linear Regression model is trained using:

```python
model.fit(X_train, y_train)
```

The model learns how advertisement spending affects sales.

---

### Step 8: Make Predictions

The trained model predicts sales values for unseen data.

```python
y_pred = model.predict(X_test)
```

---

### Step 9: Evaluate Model Performance

Two evaluation metrics are used:

### R² Score

Measures prediction quality.

Range:

* 1.0 = Perfect Prediction
* 0.0 = Poor Prediction

### Mean Absolute Error (MAE)

Measures average prediction error.

Lower MAE indicates better performance.

---

## 📈 Model Performance

Typical Results:

```text
R² Score: 0.90+

Mean Absolute Error: Approximately 1.2
```

These results indicate strong predictive performance.

---

## 📊 Sample Prediction

Input Advertising Budget:

```text
TV = 230
Radio = 37
Newspaper = 69
```

Predicted Output:

```text
Predicted Sales: 21.5
```

This means the business can expect approximately 21.5 sales units based on the given advertising budget.

---

## 📚 Learning Outcomes

Through this project, I gained practical experience in:

✅ Data Exploration

✅ Data Preprocessing

✅ Regression Analysis

✅ Linear Regression Algorithm

✅ Model Training

✅ Model Evaluation

✅ Sales Forecasting

✅ Predictive Analytics

---

## 🚀 How to Run the Project

### Install Required Libraries

```bash
pip install pandas scikit-learn
```

### Run the Script

```bash
python sales_prediction.py
```

or open the notebook in Jupyter Notebook and execute all cells.

---

## 📩 Internship Details

Internship Provider: Oasis Infobyte

Domain: Data Science

Task: Task 5 – Sales Prediction Using Python

---

## 👨‍💻 Author

Nilay Patel

Data Science Intern – Oasis Infobyte

GitHub:
https://github.com/Nilay-Patel-5

---

## 🔗 Dataset Link

https://www.kaggle.com/datasets/bumba5341/advertisingcsv

---

## ✅ Conclusion

This project successfully predicts product sales using advertisement expenditure data. By applying Linear Regression, the model learns the relationship between marketing investments and sales performance, demonstrating a practical business application of Machine Learning in sales forecasting and decision-making.
