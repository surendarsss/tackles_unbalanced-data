# tackles_unbalanced-data
Ever trained a model with 99% accuracy that fails in production?
The culprit: Imbalanced Data.
In this project, I implemented multiple strategies to handle imbalance across 4 real-world problems:

Credit Card Fraud Detection (1000:1 ratio)

Customer Churn Prediction (5:1 ratio)

Tumor Type Estimation (2:1 ratio)

Predicting Job Change (10:1 ratio)

⚠ The Problem
Most ML models favor the majority class, giving high accuracy but poor performance on minority classes.
Example: Predict “Not Fraud” every time → 99% accuracy, but 0 frauds detected.

✅ Techniques Used
✔ Class Weighting – Assign higher weight to minority classes
✔ Oversampling (SMOTE) – Generate synthetic samples for balance
✔ Undersampling – Reduce majority class size
✔ Evaluation Metrics Beyond Accuracy:

F1-Score

Precision & Recall

ROC-AUC

🔍 Tools & Libraries
Python 3.8+

scikit-learn

imbalanced-learn

NumPy, Pandas, Matplotlib

📊 Results
Baseline Accuracy: 99% (useless in real-world)

After Fix:

F1-Score: ↑ Significantly improved

AUC: ↑ High for minority class detection

