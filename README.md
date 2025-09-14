# Student Scores Prediction using Linear Regression

## Project Overview
This project is about predicting **student exam scores** based on the **number of hours they study**.  
I implemented **linear regression from scratch** using **gradient descent** to find the best fitting line that predicts scores for any given hours of study.

---

## Dataset
I created my own dataset with **20 data points**:  
- `Hours` → number of hours a student studied  
- `Scores` → marks obtained, calculated using the formula:  

Score = w * Hours + b + random_noise

markdown
Copy code

Where:  
- `w` is the score increase per hour (slope)  
- `b` is the bias (marks a student can get even if they study 0 hours)  
- `random_noise` is a small random value to simulate real-world variation  

---

## How the Model Works
1. **Predict Function**  
   - `y_hat = w * x + b` predicts the score for a given number of hours.  

2. **Cost Function**  
   - Measures how far the predicted scores are from the actual scores using Mean Squared Error.  
   - Helps us know how "wrong" the model is.

3. **Gradient Descent**  
   - Calculates the derivatives of the cost function with respect to `w` and `b`.  
   - Updates `w` and `b` step by step using a learning rate (`alpha`) to minimize the cost.  
   - Repeats until the cost stops decreasing, giving the **best w and b** for prediction.

4. **Prediction & Visualization**  
   - Once trained, the model can predict scores for any new input.  
   - Scatter plot shows actual scores, and the red line shows the best fit line (linear regression).

---

## How to Run the Code
1. Install the required Python libraries:  
   ```bash
   pip install numpy pandas matplotlib scikit-learn
Run the Jupyter notebook or Python script:

bash
Copy code
jupyter notebook Students_scores_Regression.ipynb
# OR
python Students_scores_Regression.py
You will see:

Iterations of gradient descent and cost values

Best values of w and b

Predicted score for a new input

Scatter plot with best fit line

Sample Output

Example Prediction:

Hours studied: 7

Predicted Score: 39.66

Notes
This project demonstrates the concept of linear regression, gradient descent, and model prediction.

It can be extended to multiple features (like hours, attendance, sleep hours) for multiple linear regression.

