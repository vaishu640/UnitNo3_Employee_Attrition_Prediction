# Employee Attrition Prediction Models

A machine-learning project that predicts whether an employee leaves (`LeftCompany`) using four classifiers:
- Logistic Regression
- Decision Tree
- Random Forest
- XGBoost

## Dataset
`HR_Attrition_Indian_Dataset.csv` — 5,000 rows and 22 columns. The target is `LeftCompany` (`Yes`/`No`).

## Run locally
1. Create and activate a Python virtual environment.
2. Install dependencies: `pip install -r requirements.txt`
3. Open `notebooks/employee_attrition_models.ipynb` in Jupyter.
4. Run cells from top to bottom.

## Deliverables
- Model notebook: `notebooks/employee_attrition_models.ipynb`
- Evaluation and business interpretation reports are generated in `reports/` when the notebook runs.
- Charts and model outputs are generated in `outputs/`.

## Notes
The notebook excludes `EmployeeID` and `FullName` as direct identifiers and derives `JoiningYear` from `DateOfJoining`. Model scores are generated when you run the notebook; do not claim results before execution. Results depend on package versions and runtime.

**Responsible use:** Educational prototype only. Do not use model predictions for automated hiring, firing, promotion, or other employment decisions. Validate data quality, privacy, fairness, and business context before any real-world use.
