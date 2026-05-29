# 🏥 Citizen Health Risk Analysis — Exploratory Data Analysis (EDA)


## 📌 Project Overview

This project performs a comprehensive **Exploratory Data Analysis (EDA)** on a citizen health dataset to uncover the lifestyle, demographic, and occupational factors that drive health risk scores. Using Python and its data ecosystem, the analysis examines how variables like **exercise habits, sleep duration, fast food consumption, stress levels, occupation, and country** contribute to overall health risk.

The findings are designed to help public health officials, researchers, and policy makers identify at-risk population segments and prioritise targeted health interventions.

---

## 🚨 Business Problem

> *"With rising lifestyle diseases globally, health authorities need data-driven clarity on which populations are most at risk — and what behaviours are driving that risk."*

Key questions this analysis aims to answer:

- Which **occupation groups** carry the highest average health risk?
- Does **social media usage** correlate with stress levels?
- How does **country of residence** relate to health risk scores?
- What is the impact of **weekly exercise frequency** on health risk?
- Do people who **sleep less than 6 hours** experience higher stress?
- Does **fast food frequency** elevate health risk scores?
- Which **work type** (desk job vs. other) poses the greatest risk?
- How does **age group** affect health risk — Teen, Adult, or Senior?
- Are there **gender differences** in health risk and stress levels?
- Which **single lifestyle factor** is most strongly correlated with health risk?

---

## 🔄 Project Workflow

```
Raw Data (citizen_health.xlsx)
        │
        ▼
 Data Loading & Initial Inspection
  └── df.head(), df.shape, df.info(), df.describe()
        │
        ▼
 Data Cleaning
  ├── Removed duplicate citizen records (subset='citizen_id')
  ├── Filled nulls: work_type (mode), exercise_days_per_week (mean), fast_food_frequency (mode)
  ├── Split combined column 'occupation and income_level' into two separate columns
  ├── Standardised diet_type values ("Vegan" → "Veg")
  └── Created age_category bins: Teen (18–26), Adult (27–60), Senior (61+)
        │
        ▼
 Exploratory Data Analysis (10 Business Questions)
  └── groupby aggregations, correlation matrix, bar plots
        │
        ▼
 Observations & Conclusions
```

---

## 🛠️ Tools & Libraries Used

| Tool / Library | Purpose |
|---|---|
| **Python 3** | Core programming language |
| **Pandas** | Data loading, cleaning, transformation, and aggregation |
| **Matplotlib** | Base plotting framework |
| **Seaborn** | Statistical visualisations (bar plots, correlation) |
| **Jupyter Notebook** | Interactive analysis environment |

---

## 📂 Dataset

- **File:** `citizen_health.xlsx`
- **Key Columns:** `citizen_id`, `age`, `gender`, `country`, `occupation`, `income_level`, `work_type`, `diet_type`, `exercise_days_per_week`, `sleep_hours`, `fast_food_frequency`, `social_media_hours`, `stress_level`, `health_risk_score`
- **Derived Columns:** `age_category` (Teen / Adult / Senior), `occupation` and `income_level` (split from a combined column)

> **Note:** The dataset contains citizen-level health and lifestyle records from multiple countries, covering demographics, daily habits, and health outcomes.

---

## 🔍 Analysis Questions & Key Findings

### 1. 🏢 Occupation vs. Health Risk Score
> *Which occupation group has the highest average health risk score?*

**Finding:** Journalists have the highest average health risk score, followed closely by Labourers — indicating that both mentally demanding and physically strenuous occupations elevate health risk.

---

### 2. 📱 Social Media Hours vs. Stress Level
> *Is there a relationship between social media usage and stress level?*

**Finding:** Correlation analysis shows **no meaningful relationship** between social media hours and stress levels in this dataset.

---

### 3. 🌍 Country vs. Health Risk Score
> *What is the average health risk score by country?*

**Finding:** **South Korea** has the highest average health risk score, followed by **Germany**, **UAE**, and **South Africa** — suggesting regional lifestyle or environmental risk factors worth investigating further.

---

### 4. 🏃 Exercise Frequency vs. Health Risk Score
> *How does exercise days per week impact health risk?*

**Finding:** Citizens exercising **all 7 days a week** show a noticeably **lower health risk score** — confirming a clear protective effect of regular physical activity.

---

### 5. 😴 Sleep Hours vs. Stress Level
> *Do people who sleep less than 6 hours have higher stress levels?*

**Finding:** Citizens sleeping **6 hours or less** exhibit **higher average stress levels** compared to those who sleep more — reinforcing the well-documented link between sleep deprivation and stress.

---

### 6. 🍔 Fast Food Frequency vs. Health Risk Score
> *Does fast food consumption affect health risk scores?*

**Finding:** Higher fast food consumption is directly associated with **elevated health risk scores** — those who eat fast food most frequently carry the greatest risk.

---

### 7. 💼 Work Type vs. Health Risk Score
> *Which work type has the highest health risk?*

**Finding:** **Desk job** workers have the highest health risk score across all work types — likely due to sedentary behaviour, highlighting the need for workplace wellness programmes.

---

### 8. 👴 Age Category vs. Health Risk Score
> *How does age group affect health risk score?*

**Finding:** **Senior citizens (60+)** have the highest health risk scores, followed by Adults, then Teens — consistent with the natural increase in health vulnerability with age.

---

### 9. ⚧ Gender vs. Health Risk Score
> *Do health risks differ across genders?*

**Finding:** **Female citizens** show a slightly higher average health risk score than male citizens in this dataset.

---

### 10. 🔗 Strongest Lifestyle Factor Correlation
> *Which lifestyle factor impacts health the most?*

**Finding:** **Stress level** is the most strongly correlated variable with health risk score — making it the single most impactful lifestyle factor in this dataset.

---

## 📝 Conclusion

| Finding | Key Takeaway |
|---|---|
| 🏢 Occupation | Journalists & Labourers face the highest health risk |
| 🌍 Country | South Korea, Germany, UAE lead in health risk |
| 🏃 Exercise | Daily exercise significantly lowers health risk |
| 😴 Sleep | Less than 6 hours sleep raises stress levels |
| 🍔 Fast Food | Higher frequency directly raises health risk |
| 💼 Work Type | Desk job workers carry the most risk |
| 👴 Age | Seniors are the most at-risk age group |
| ⚧ Gender | Females show slightly higher health risk scores |
| 🔗 Correlation | Stress level is the strongest predictor of health risk |

---

## ✅ Recommendations

1. **Workplace wellness programmes** — Especially for desk-job workers and journalists; standing desks, movement breaks, and mental health support can directly reduce risk.
2. **Promote daily exercise** — Even light daily activity shows measurable impact on reducing health risk scores.
3. **Sleep health campaigns** — Public health messaging should emphasise 7–8 hours of sleep as a stress-reduction and risk-reduction tool.
4. **Dietary interventions** — Reduce fast food access or incentivise healthier food choices in high-risk occupation groups.
5. **Country-specific strategies** — South Korea, Germany, and UAE should be prioritised for targeted public health initiatives based on their elevated risk scores.
6. **Stress management as a primary intervention** — Given stress is the strongest correlated factor, mental health resources should be the first line of public health investment.

---

## 📁 Project Structure

```
citizen-health-analysis/
│
├── health_analysis.ipynb    
├── citizen_health.xlsx       
├── README.md                

```

---

## 🧠 Skills Demonstrated

- ✅ Data loading from Excel using Pandas
- ✅ Duplicate detection and removal
- ✅ Null value imputation (mode, mean strategies)
- ✅ String splitting and column engineering
- ✅ Value standardisation and category mapping
- ✅ Age binning with `pd.cut()` for derived features
- ✅ GroupBy aggregations for multi-dimensional analysis
- ✅ Correlation matrix analysis for feature relationships
- ✅ Statistical bar chart visualisation with Seaborn
- ✅ Translating EDA findings into actionable public health insights

---

## 👤 Author

**Sachin**
*Data Analyst | Python EDA Specialist | Public Health Analytics*

# 🔗 Connect With Me

- LinkedIn: www.linkedin.com/in/sachindevarajan

> *"The goal is to turn data into information, and information into insight." — Carly Fiorina*

---

⭐ **Found this useful? Give it a star** — it helps others discover the project and encourages more open analytics work!
