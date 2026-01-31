# Employee Turnover Prediction

## Overview
This project builds an end-to-end supervised machine learning pipeline to predict employee attrition using structured HR data. The objective is to identify key drivers of turnover and support data-driven employee retention strategies.

---

## Dataset
The dataset contains numerical and categorical employee attributes such as satisfaction level, workload, tenure, department, and salary.

- **Target variable:** `quit` (0 = Stayed, 1 = Left)

---

## Approach
- Performed exploratory data analysis to understand turnover patterns
- Preprocessed data using `ColumnTransformer` and `Pipeline` to prevent data leakage
- Compared Logistic Regression, Decision Tree, and Random Forest models
- Evaluated models using ROC–AUC, precision, recall, and confusion matrices

---

## Results
| Model | ROC–AUC | Precision (Quit) | Recall (Quit) |
|------|--------|-----------------|---------------|
| Logistic Regression | 0.85 | 0.45 | 0.84 |
| Decision Tree | 0.96 | 0.73 | 0.95 |
| Random Forest | **0.99** | **0.93** | **0.93** |

**Random Forest** was selected as the final model due to its strong and balanced performance.

---

## Key Insights
- Employee satisfaction is the strongest predictor of turnover
- Turnover risk increases after 3–5 years of tenure
- Both overworked and underutilized employees are more likely to leave

---

## Tech Stack
Python, pandas, scikit-learn, seaborn, matplotlib

---

## Project Structure
<pre>
├── Analysis.ipynb
├── EmployeeTurnover.ipynb
├── employee_data.csv
└── README.md
</pre>
