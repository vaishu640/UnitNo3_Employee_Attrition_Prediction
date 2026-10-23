# Business Interpretation Report: Employee Attrition Prediction

## Dataset overview
- Records used: 5,000
- Input features after removing direct identifiers: 19
- Observed attrition rate: 37.10%
- Target definition: LeftCompany = Yes means the employee left.

## Model selection
The best model by held-out test ROC-AUC in this run was **Random Forest**.
The final metrics are available in `../outputs/tuned_model_comparison.csv`.
Use precision and recall alongside accuracy because the costs of missed attrition and false alerts differ.

## Features to investigate
The top features by permutation importance for this model are: JobSatisfaction, WorkLifeBalance, AppraisalRating, DoesOvertime, YearsWithCompany.
Permutation importance indicates predictive usefulness in this dataset; it does not prove that a feature causes attrition.

## Suggested HR actions
1. Use model outputs only to guide voluntary, aggregate retention analysis and employee listening—not automated employment decisions.
2. Investigate whether the most predictive factors are actionable and supported by qualitative evidence.
3. Compare error rates and calibration across relevant employee groups before any operational use.
4. Recheck performance on newer data and monitor for drift.

## Limitations
- Dataset patterns may not represent a real organization or future workforce.
- Predictive associations are not causal explanations.
- The model can reflect historical bias and data collection issues.
- Any real deployment requires privacy review, fairness evaluation, and HR/legal oversight.
