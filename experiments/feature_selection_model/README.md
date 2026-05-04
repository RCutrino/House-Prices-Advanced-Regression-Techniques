# Feature Selection Experiment

## Objective
Test whether applying SelectFromModel with ElasticNet improves generalization performance compared to the baseline model.

---

## Methodology
- Same preprocessing pipeline as baseline
- Feature selection using ElasticNet-based SelectFromModel
- Final model: ElasticNet regression
- Evaluation: Kaggle RMSE

---

## Results

| Model | Kaggle RMSE |
|------|-------------|
| Baseline (no feature selection) | 0.13408 |
| With feature selection | 0.13529 |

---

## Conclusion
Feature selection did not improve performance.  
ElasticNet already performs implicit regularization, making external feature selection redundant in this case.

Therefore, the baseline model was retained as the final submission model.

---

## Key Insight
In regularized linear models, additional feature selection may reduce performance by removing weakly informative but useful correlated features.
