# Student Scores Prediction using Linear Regression

[![Python](https://img.shields.io/badge/python-3.11-blue)](https://www.python.org/)

---

## Project Overview
Predict **student exam scores** based on **hours of study** using **linear regression** implemented from scratch with **gradient descent**.

---

## Dataset
I created a dataset with **20 data points**:

| Hours | Score |
|-------|-------|
| 1.5   | 12    |
| 2     | 15    |
| ...   | ...   |

- **Hours** → number of study hours  
- **Scores** → marks obtained  
- Formula: `Score = w * Hours + b + random_noise`

---

## How the Model Works

1. **Predict Function:** `y_hat = w * x + b`  
2. **Cost Function:** Measures error using **Mean Squared Error**  
3. **Gradient Descent:** Updates `w` and `b` to minimize cost  
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

Hours studied: 7

Predicted Score: 39.66

Notes
Demonstrates linear regression, gradient descent, and predictions

Can be extended to multiple features for multiple regression
