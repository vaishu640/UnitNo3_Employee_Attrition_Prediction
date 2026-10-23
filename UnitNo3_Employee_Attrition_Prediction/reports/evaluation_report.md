# Evaluation Report: Employee Attrition Prediction

## Baseline model comparison

| Model               |   Accuracy |   Precision |   Recall |     F1 |   ROC-AUC |
|:--------------------|-----------:|------------:|---------:|-------:|----------:|
| Random Forest       |      0.781 |      0.7923 |   0.5553 | 0.6529 |    0.7514 |
| Decision Tree       |      0.741 |      0.6739 |   0.5849 | 0.6263 |    0.6947 |
| Logistic Regression |      0.643 |      0.5148 |   0.6577 | 0.5775 |    0.6932 |

## Tuned model comparison

| Model               |   Accuracy |   Precision |   Recall |     F1 |   ROC-AUC |
|:--------------------|-----------:|------------:|---------:|-------:|----------:|
| Random Forest       |      0.782 |      0.7684 |   0.5903 | 0.6677 |    0.7567 |
| Decision Tree       |      0.78  |      0.7849 |   0.5606 | 0.6541 |    0.751  |
| Logistic Regression |      0.644 |      0.5161 |   0.6496 | 0.5752 |    0.6951 |

## Cross-validation results

| Model               |   accuracy_mean |   precision_mean |   recall_mean |   f1_mean |   roc_auc_mean |   accuracy_std |   precision_std |   recall_std |   f1_std |   roc_auc_std |
|:--------------------|----------------:|-----------------:|--------------:|----------:|---------------:|---------------:|----------------:|-------------:|---------:|--------------:|
| Random Forest       |          0.8    |           0.8251 |        0.5849 |    0.684  |         0.7706 |         0.011  |          0.0129 |       0.0329 |   0.0235 |        0.0173 |
| Decision Tree       |          0.7397 |           0.6645 |        0.6085 |    0.6345 |         0.7206 |         0.0181 |          0.0336 |       0.0238 |   0.0191 |        0.0149 |
| Logistic Regression |          0.6468 |           0.5191 |        0.6475 |    0.5759 |         0.701  |         0.0048 |          0.0047 |       0.0339 |   0.0147 |        0.0108 |

## Notes
- Test set was held out from model tuning.
- CV used stratified 5-fold splits on training data.
- ROC-AUC measures ranking performance, not probability calibration.
