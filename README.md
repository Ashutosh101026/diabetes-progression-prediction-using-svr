# Diabetes Progression Prediction using Support Vector Regression (SVR)

## Project Overview

This project implements a Support Vector Regression (SVR) model to predict diabetes disease progression using medical features from the Scikit-Learn Diabetes dataset.

The project demonstrates regression modeling, feature preprocessing, kernel comparison, hyperparameter tuning using GridSearchCV, and model evaluation using R² Score.

---

## Problem Statement

The objective of this project is to predict the progression of diabetes disease based on patient medical measurements using a machine learning regression approach.

---

## Dataset Information

**Dataset:** Diabetes Dataset

**Source:** Scikit-Learn Built-in Dataset

**Samples:** 442

**Features:** 10

### Features

- Age
- Sex
- Body Mass Index (BMI)
- Blood Pressure
- Serum Measurements

### Target Variable

- Diabetes Disease Progression Score

---

## Project Workflow

## 1. Data Loading

- Loaded Diabetes dataset using Scikit-Learn.
- Converted dataset into Pandas DataFrame.

---

## 2. Data Exploration

Performed:

- Dataset shape checking
- Missing value analysis
- Feature and target inspection

---

## 3. Data Preparation

Separated:

- Independent variables (X)
- Target variable (y)

Performed train-test split:

- Training Data: 70%
- Testing Data: 30%

---

## 4. Feature Scaling

Applied StandardScaler on the target variable to normalize values before training the SVR model.

---

## 5. Model Development

Implemented:

```python
SVR()
```

Support Vector Regression model from Scikit-Learn.

---

## 6. Kernel Comparison

Different SVR kernels were tested:

### RBF Kernel

```python
SVR(kernel="rbf")
```

### Linear Kernel

```python
SVR(kernel="linear")
```

### Polynomial Kernel

```python
SVR(kernel="poly")
```

The performance of each kernel was compared using R² Score.

---

## 7. Hyperparameter Tuning

GridSearchCV was applied to find the best SVR configuration.

Parameters tuned:

```python
C = [1,2,5,10,50,100]

kernel = ["rbf","linear","poly"]

epsilon = [0.01,0.1,0.2,0.3]
```

5-fold cross-validation was used during hyperparameter optimization.

The best parameters were selected based on R² score.

---

## 8. Model Evaluation

The model performance was evaluated using:

- R² Score

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-Learn
- Jupyter Notebook
- Matplotlib
- Seaborn

---

## Machine Learning Algorithm

## Support Vector Regression (SVR)

SVR is a supervised machine learning algorithm used for predicting continuous values.

Advantages:

- Handles nonlinear relationships
- Effective with high-dimensional data
- Uses kernel functions for complex patterns
- Controls model complexity using regularization

---

## Results

Different SVR kernels were compared and hyperparameter tuning was performed using GridSearchCV to identify the best-performing model configuration.

The optimized SVR model improved prediction performance by selecting suitable values of C, kernel type, and epsilon.

---

## Learning Outcomes

Through this project, I learned:

- Regression Problems
- Support Vector Regression
- Kernel Selection
- Feature Scaling
- Hyperparameter Optimization
- GridSearchCV
- Cross Validation
- Regression Model Evaluation

---

## Installation

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

---

## Run Project

```bash
jupyter notebook
```

Open:

```text
SVR_ON_DIABETES_DATASET.ipynb
```

---

## Project Structure

```text
diabetes-progression-prediction-using-svr
│
├── SVR_ON_DIABETES_DATASET.ipynb
├── README.md
└── requirements.txt
```

---

## Future Improvements

- Compare with Random Forest Regression
- Compare with XGBoost Regression
- Deploy model using Streamlit
- Add visualization dashboard
- Perform feature importance analysis

---

## Author

Ashutosh Mehta

Computer Engineering Student

Machine Learning Enthusiast
