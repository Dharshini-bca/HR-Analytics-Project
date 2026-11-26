# HR Analytics: Employee Experience, Performance & Training

## Project overview
An exploratory HR analytics project using Python to examine employee status, performance ratings, employee survey scores, and training outcomes/costs.

## Dataset
- 2,845 employee-related records and 28 columns in the original source file.
- The public copy in `data/hr_analytics_anonymized.csv` removes direct identifiers and selected sensitive/personal fields (employee ID, date of birth, state, race, gender, marital status, and raw employment/survey/training dates).
- The source file was named `sales data.csv`, but its fields describe HR and employee training data.

## Questions explored
1. How are active and terminated records distributed?
2. Which performance score category is most common?
3. Which departments have the largest number of records?
4. What are the average engagement, satisfaction, and work-life balance scores?
5. How are training outcomes and training costs distributed?

## Tools
Python, pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook.

## Repository structure
```text
HR-Analytics/
├── HR_Analytics_Analysis.ipynb
├── HR_Analytics_Project_Summary.pptx
├── README.md
├── requirements.txt
├── data/
│   └── hr_analytics_anonymized.csv
└── images/
    ├── employee_status.png
    ├── performance_score.png
    ├── department.png
    ├── training_outcomes.png
    ├── survey_scores.png
    └── training_cost_by_outcome.png
```

## Key descriptive findings
- 2,845 records.
- Active: 2,458 (86.4%); Terminated: 387 (13.6%).
- Fully Meets: 2,251 records (79.1%).
- Production is the largest department group: 1,910 records.
- Average engagement: 2.94/5; satisfaction: 3.03/5; work-life balance: 2.99/5.
- Training outcomes: Completed 737, Incomplete 731, Passed 709, Failed 668.
- Total recorded training cost: 1,591,148.63 (currency not specified in source).

## Important scope and limitations
This is descriptive exploratory analysis, not an attrition prediction model. The source does not provide exit reasons, so it cannot support claims about why employees leave. Currency and data dictionary definitions were not supplied. Survey score averages are interpreted on the observed 1–5 scale.

## Run locally
```bash
pip install -r requirements.txt
jupyter notebook HR_Analytics_Analysis.ipynb
```
