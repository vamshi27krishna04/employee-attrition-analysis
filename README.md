# Employee Attrition Prediction

Machine learning analysis predicting employee turnover among knowledge workers using Random Forest and XGBoost ensemble methods. Compares bagging vs. gradient boosting approaches with cross-validation on IBM HR Analytics dataset.

## Research Question
What combination of work-life balance factors, compensation metrics, and career progression indicators best predicts employee attrition, and which employees are at highest risk of leaving?

## Dataset
- Source: IBM HR Analytics Employee Attrition Dataset (Kaggle)
- Size: 1,470 employees, 35 features
- Outcome: Attrition (Yes/No) - 16.1% positive class

## Methods
Two ensemble models compared:
1. Random Forest (Bagging) - Bootstrap aggregating with 200 trees
2. XGBoost (Gradient Boosting) - Sequential trees with L1/L2 regularization

## Key Results
| Metric | Random Forest | XGBoost |
|--------|--------------|---------|
| Recall | 0.337 | **0.416** |
| ROC-AUC | 0.799 | 0.797 |
| F1-Score | 0.432 | **0.505** |

Final Model: XGBoost (selected for superior recall)

