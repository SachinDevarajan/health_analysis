# Citizen Health Risk Analysis using Python (EDA)

This project is an Exploratory Data Analysis (EDA) of citizen health and lifestyle data using Python, Pandas, Matplotlib, and Seaborn.

I built this project to understand how lifestyle habits, occupation, age, sleep, exercise, and stress levels are related to health risk scores. The analysis uses data cleaning, visualization, and statistical methods to identify patterns and useful insights.

## About the Dataset

The project uses a citizen health dataset containing information such as:

- Age and gender
- Country and occupation
- Income level and work type
- Exercise frequency
- Sleep duration
- Diet and fast food consumption
- Social media usage
- Stress level and health risk score

## Technologies Used

- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook
- Exploratory Data Analysis (EDA)

## Project Workflow

1. Load and explore the Excel dataset using Pandas.
2. Remove duplicate records and handle missing values.
3. Clean and standardize column values.
4. Split occupation and income information into separate columns.
5. Create age categories for analysis.
6. Analyze relationships between lifestyle factors and health risk.
7. Create visualizations using Matplotlib and Seaborn.
8. Identify patterns and summarize key findings.

## Key Analysis and Findings

- **Occupation:** Journalists and labourers have the highest average health risk scores.
- **Exercise:** People exercising seven days a week show lower health risk scores.
- **Sleep:** People sleeping six hours or less have higher average stress levels.
- **Fast Food:** Frequent fast food consumption is associated with higher health risk scores.
- **Work Type:** Desk job workers show the highest average health risk.
- **Age:** Senior citizens have higher health risk scores compared to younger age groups.
- **Gender:** Female citizens show slightly higher average health risk scores.
- **Country:** South Korea has the highest average health risk score in the dataset.
- **Social Media:** No meaningful correlation was found between social media usage and stress.
- **Stress:** Stress level has the strongest correlation with health risk score among the lifestyle factors analyzed.

These findings show associations within the dataset and do not necessarily establish cause and effect.

## Project Structure

```text
citizen-health-analysis/
│
├── health_analysis.ipynb
├── citizen_health.xlsx
└── README.md
```

## How to Run

**1. Install the required libraries**

```bash
pip install pandas openpyxl matplotlib seaborn notebook
```

**2. Open the Jupyter Notebook**

```bash
jupyter notebook health_analysis.ipynb
```

**3. Run the notebook cells**

Make sure `citizen_health.xlsx` is in the project folder before running the analysis.

## What I Learned

Through this project, I gained practical experience in:

- Data cleaning and preprocessing using Pandas
- Handling missing values and duplicate records
- Feature engineering and age categorization
- GroupBy operations and data aggregation
- Correlation analysis
- Data visualization using Matplotlib and Seaborn
- Exploratory Data Analysis
- Identifying insights from real-world-style datasets

## Author

**Sachin Devarajan**

GitHub: [SachinDevarajan](https://github.com/SachinDevarajan)

LinkedIn: [Sachin Devarajan](https://www.linkedin.com/in/sachindevarajan)
