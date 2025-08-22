# Ridge vs Lasso Regression

This project explores two important regularization techniques in machine learning: **Ridge Regression** and **Lasso Regression**. Both methods are extensions of linear regression that help control overfitting and improve model generalization by applying a penalty to the size of coefficients.

---

## 1. Why Regularization?
When a model has too many features or multicollinearity, ordinary linear regression tends to overfit the training data. Regularization methods add a penalty to the loss function, forcing the model to keep coefficients small and avoid overly complex patterns.

---

## 2. Ridge Regression (L2 Regularization)
- **Penalty:** Sum of the squared values of the coefficients (L2 norm).  
- **Effect:** Shrinks coefficients towards zero but **never makes them exactly zero**.  
- **Best for:** Situations where all features are useful, especially when features are correlated.  
- **Intuition:** Think of Ridge as spreading the "weight" across all features rather than ignoring any completely.

---

## 3. Lasso Regression (L1 Regularization)
- **Penalty:** Sum of the absolute values of the coefficients (L1 norm).  
- **Effect:** Shrinks some coefficients exactly to zero, effectively performing **feature selection**.  
- **Best for:** Datasets with many irrelevant features where we want a simpler, sparse model.  
- **Intuition:** Lasso automatically chooses the most important features by dropping less useful ones.

---

## 4. Key Differences
| Aspect | Ridge | Lasso |
|--------|-------|-------|
| Penalty Type | L2 (squared coefficients) | L1 (absolute coefficients) |
| Coefficients | Small but non-zero | Some exactly zero |
| Use Case | Good with correlated features | Good for feature selection |
| Model Complexity | Keeps all features | Produces sparse models |

---

## 5. Practical Insights
- **Ridge** is safer when you suspect all predictors contribute to the outcome.  
- **Lasso** is useful when you believe only a few predictors are truly important.  
- **Elastic Net** (a mix of Ridge and Lasso) is often used to combine their strengths.  

---

## 6. Conclusion
- Both Ridge and Lasso help prevent overfitting and improve generalization.  
- Ridge balances weights smoothly across features, while Lasso encourages sparsity.  
- Choosing between them depends on the dataset and the problem requirements.  
