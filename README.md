# Regression Modeling and Performance Evaluation – Coffee Sales Data

##  Dataset Summary
The dataset `index_1` contains 3636 rows and 6 columns, capturing customer coffee transactions. It includes:
- `date`: Purchase date
- `datetime`: Full timestamp of the transaction
- `cash_type`: Payment method (only "card" in this dataset)
- `card`: Unique anonymous customer identifier
- `money`: Amount spent
- `coffee_name`: Type of coffee purchased

##  Modeling Process
- Feature engineering: Extracted features like hour of purchase, day of week, coffee type encoding.
- Regression Models Built:
  1. **Linear Regression**
  2. **Ridge Regression**
- Model evaluation metrics:
  - R-squared (R²)
  - Mean Squared Error (MSE)
  - Root Mean Squared Error (RMSE)
  - Cross-validation scores

##  Insights
- The time of day and type of coffee significantly impact the money spent.
- Ridge Regression slightly outperformed Linear Regression in generalization.
- Customer behavior patterns could be inferred by time and coffee preference.

##  Challenges
- All payments are via card; no variation in `cash_type`.
- Highly repetitive transactions (multiple identical purchases).
- Dealt with categorical encoding for `coffee_name` and time extraction from `datetime`.

##  Conclusion
Regularization (Ridge) helped reduce overfitting. With further data (e.g., customer profiles or loyalty), predictions could be refined further.

