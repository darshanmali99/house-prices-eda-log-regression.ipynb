## 🔄 Log Transformation Improvement

After establishing a baseline Linear Regression model, the target variable (`SalePrice`) was log-transformed to reduce right skewness and stabilize variance.

### Why Log Transformation?
- House prices are heavily right-skewed
- Linear Regression performs better with normally distributed targets
- RMSE penalizes large errors more strongly for expensive houses

### What Changed
- Trained the model on `log(SalePrice)`
- Converted predictions back using `expm1`
- Improved model generalization without changing the algorithm

### 📈 Impact
- Baseline Rank: **5541**
- After Log Transformation: **4995**
- Improvement achieved through better data representation, not model complexity

## 🔗 Competition & Profile Links
- Kaggle Competition: House Prices – Advanced Regression Techniques
- Kaggle Profile: https://www.kaggle.com/darshanmali99
