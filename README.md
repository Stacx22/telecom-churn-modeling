Telecom Customer Churn Modeling

```markdown
# Telecom Customer Churn Modeling

Predictive model to identify customers likely to cancel service, enabling proactive retention strategies.

### Data
- Telecom service usage + customer attributes

### Methods
- Logistic Regression & Random Forest
- SMOTE sampling for imbalance
- Metrics: ROC AUC & F1 Score

### Results
| Model | F1 Score | ROC AUC |
|------|---------|---------|
| Logistic Regression | 0.72 | 0.78 |
| Random Forest | 0.81 | 0.87 |

> See `docs/Telecom_Churn_Results_and_Illustrations.pdf` for charts

### Key Drivers
- Customer service calls
- Daytime minutes
- Monthly charge

---
