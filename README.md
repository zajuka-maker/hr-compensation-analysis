# HR Compensation Analysis | Python & Pandas

An educational HR analytics project covering data quality assessment, data cleaning, salary analysis, and A/B test planning.

## Project goal

Transform inconsistent employee records into a documented, analysis-ready dataset and prepare salary summaries for HR reporting.

## Tools

- Python
- Pandas and NumPy
- OpenPyXL
- Statsmodels
- Google Colab / Jupyter Notebook

## Analysis workflow

1. Inspect missing values, duplicates, data types, and inconsistent categories.
2. Validate employee IDs, salaries, hire dates, and performance scores.
3. Standardize categories using reference tables.
4. Prepare a cleaned dataset while retaining original values for audit.
5. Calculate salary summaries by department, city, gender, and job title.
6. Identify salary outliers using IQR and compare salaries with job averages.
7. Export cleaned data, summary tables, and a cleaning report to Excel and CSV.

Salary summaries use active employees with valid salaries who meet the notebook's inclusion rules.

## Data cleaning

The source dataset contains 200 rows. After removing one full duplicate, the cleaned dataset contains 199 rows.

The notebook documents cleaning rules, affected records, assumptions, and quality checks. Salary outliers are flagged for review; an outlier alone does not establish a data error.

## A/B test planning

The notebook includes a proposed experiment comparing two employee onboarding formats.

- Primary metric: probation pass rate
- Baseline: 77%
- Target: 85%
- Significance level: 5%
- Statistical power: 80%
- Allocation: 50/50
- Estimated sample: 374 participants per group, 748 in total

At 25 new hires per month, recruitment would take approximately 30 months, plus the observation period for the final cohort. The plan discusses feasibility, seasonality, group balance, and other risks.

This section is an experiment plan, not the result of a completed A/B test.

## Notebook

[View the analysis notebook](HR_Compensation_Analysis_Nataliia_Snihova.ipynb)

## How to run

1. Open the notebook in Google Colab.
2. Run the first code cell and upload `HR_Compensation_Raw_Data_200_rows.xlsm`.
3. Run the remaining cells in order.

Required worksheets:
- `employees_raw`
- `reference_tables`
- `cleaning_report_template`

Required Python packages: pandas, numpy, openpyxl, and statsmodels.

The source workbook is required to reproduce the analysis. Saved outputs are included in the notebook for review.

## Author

**Nataliia Snihova**

---

## Українською

Навчальний проєкт з HR-аналітики: перевірка якості та очищення даних працівників, аналіз зарплат і планування A/B-тесту нового формату адаптації.

У Python/Pandas виконано стандартизацію категорій, обробку зарплат і дат, перевірку дублікатів та пропусків, розрахунок показників за відділами, містами, статтю й посадами.

Результат — очищений набір даних, підсумкові таблиці та звіт про очищення. Окремий блок містить гіпотези A/B-тесту, розрахунок вибірки, тривалості та аналіз ризиків.
