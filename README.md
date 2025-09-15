# Student Scores Prediction using Linear Regression

[![Python](https://img.shields.io/badge/python-3.11-blue)](https://www.python.org/)

---

## Project Overview
Predict **student exam scores** based on **hours of study** using **linear regression** implemented from scratch with **gradient descent**.

This project demonstrates how a simple supervised machine learning model can predict outcomes based on a single feature.

---

## Dataset
The dataset is downloaded from [Kaggle: Student Scores](https://www.kaggle.com/datasets/kamleshsam/student-scores) and contains **25 data points**:

| Hours | Scores |
|-------|--------|
| 2.5   | 21     |
| 5.1   | 47     |
| 3.2   | 27     |
| ...   | ...    |

- **Hours** → number of study hours  
- **Scores** → marks obtained  
- The dataset is in **CSV format** (`student_scores.csv`)  
- It can be loaded directly using `pandas.read_csv()`

---

## How the Model Works

1. **Predict Function:** `y_hat = w * x + b`  
2. **Cost Function:** Measures error using **Mean Squared Error**  
3. **Gradient Descent:** Updates `w` and `b` iteratively to minimize cost  
4. **Prediction & Visualization:**  
   - Scatter plot: actual scores  
   - Red line: best fit linear regression  

---

## How to Run
```bash
pip install numpy pandas matplotlib scikit-learn
jupyter notebook Students_scores_Regression.ipynb
# OR
python Students_scores_Regression.py
Example Output:

yaml
Copy code
Hours studied: 7
Predicted Score: 67.37
Notes
Demonstrates linear regression, gradient descent, and predictions

Can be extended to multiple features for multiple regression

Dataset can be updated easily without changing the code
