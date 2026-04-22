# HR-Attrition-Analysis
# SQL Project 




## 🔥 HR Attrition Analytics in SQL — uncover why employees leave and what it costs  
From churn drivers to $3.4M impact: turning HR data into retention strategy.

---

# 👥 HR Attrition & Retention Analytics  
### *SQL Analytics Project | Employee Churn, Cost of Attrition & Retention Drivers*

---

## 📌 Overview
This project analyzes HRIS data to uncover **why employees leave, where attrition hits hardest, and its financial impact**.

Using SQL Server, I built an end-to-end attrition diagnostic system covering:
- 📊 Baseline KPIs  
- 🔍 Department & role hotspots  
- ⚠️ Burnout & satisfaction signals  
- 📉 Promotion stagnation  
- 🧠 Manager impact  
- 💰 Cost of employee churn  

➡️ The outcome: a **data-driven retention strategy + actionable HR insights**

---

## 🎯 Objective
Quantify company-wide attrition, identify root causes, and translate employee churn into **financial impact** to support strategic retention decisions.

---

## 🚀 Key Goals
- 📏 **Measure Baseline** – Attrition rate, headcount, cost per leaver  
- 🔥 **Find Hotspots** – Departments & roles with highest turnover  
- 🧪 **Test Drivers** – Overtime, promotion gaps, satisfaction, commute  
- 📚 **Evaluate Training ROI** – Does L&D reduce churn?  
- 💸 **Quantify Loss** – Annual cost of attrition  
- ⚡ **Enable Action** – Risk scoring + HR intervention list  

---

## 🧠 Skills Demonstrated

| Category            | Skills |
|--------------------|-------|
| 💻 SQL Server       | CTEs, Window Functions, `SUM() OVER`, `PERCENTILE_CONT`, CASE Logic |
| 👥 People Analytics | Attrition Rate, Tenure Analysis, Satisfaction Modeling |
| 📊 Analytics        | Segmentation, Risk Scoring, Lift Analysis |
| 💼 Business Thinking| ROI Framing, HR Strategy, Executive Insights |
| 🧹 Data Quality     | NULL Handling, Filtering (HAVING), Metric Consistency |

---

## 🗂️ Data Overview

**Table:** `hr_data`  
**Grain:** One row per employee  
**Size:** ~1,400 – 15,000 rows  

### Key Fields

| Column | Type | Description |
|--------|------|------------|
| emp_no | INT | Employee ID |
| attrition | VARCHAR | Yes/No |
| department, job_role | VARCHAR | Org structure |
| age, gender, marital_status | Mixed | Demographics |
| monthly_income | INT | Salary |
| overtime | VARCHAR | Yes/No |
| years_at_company | INT | Tenure |
| years_since_last_promotion | INT | Career growth |
| job_satisfaction | INT (1–4) | Survey |
| work_life_balance | INT (1–4) | Survey |
| distance_from_home | INT | Commute |
| training_times_last_year | INT | L&D |
| years_with_current_manager | INT | Manager stability |

---

## 🔧 Data Transformation
Key transformations performed in SQL:

- 🏷️ Attrition flag (`Yes = 1`)  
- 📊 Tenure & salary banding  
- 🔄 Satisfaction pivot using `UNION ALL`  
- 🚗 Commute grouping (distance buckets)  
- ⚠️ Risk score based on 6 churn drivers  
- 💰 Cost of attrition (0.5 × annual salary)

---

## 🏗️ Data Modeling

Structured into 3 logical layers:

1. **Staging** – Clean, filter, create derived columns  
2. **Metrics** – Aggregate KPIs by segment  
3. **Insights** – Compare vs baseline (lift analysis)

✔️ Fully reusable & refreshable monthly  

---

## 🔍 Analysis Breakdown

| # | Business Question | Method |
|--|------------------|--------|
| 1 | Attrition rate & headcount | COUNT, SUM, AVG |
| 2 | Worst departments/roles | GROUP BY + HAVING |
| 3 | Overtime impact | Segment comparison |
| 4 | Promotion stagnation | Cross analysis (tenure × salary) |
| 5 | Satisfaction drivers | Pivot + attrition rates |
| 6 | Commute/travel effect | Distance bands |
| 7 | Training ROI | Attrition by training count |
| 8 | Manager impact | Tenure with manager |
| 9 | Cost of attrition | Salary-based estimation |

📂 SQL queries stored in `/sql/` with business context comments.

---

## 💡 Key Insights & Recommendations

### ⚠️ 1. Overtime = High Churn
- 31% attrition vs 8% (no overtime)  
✔️ Cap overtime or introduce premium pay  

---

### 📉 2. Promotion Delays Drive Exit
- 42% churn after 4+ years without promotion  
✔️ Introduce **3-year promotion review policy**

---

### 😓 3. Work-Life Balance is #1 Predictor
- 47% churn at lowest score  
✔️ Shift to **monthly pulse surveys**

---

### 🚗 4. Commute + Travel = Exit Trigger
- 51% churn (long distance + frequent travel)  
✔️ Remote options or travel incentives  

---

### 📚 5. Training Reduces Attrition
- 26% churn (0–1 training) → 9% (2+)  
✔️ Make **2 trainings/year mandatory**

---

### 👨‍💼 6. New Managers Increase Risk
- 34% churn under new managers  
✔️ Add **90-day onboarding + skip-level reviews**

---

### 💰 7. Financial Impact
- Total attrition cost: **$3.4M**  
✔️ $200K retention budget breaks even at **6% improvement**

---

## 📊 Conclusion

Attrition is **predictable and preventable**.

Key risk combinations:
- Overtime + early tenure  
- Promotion stagnation + low pay  
- Long commute + travel  
- New manager transitions  

### 💼 Business Impact:
- Identified a **$3.4M problem**
- Proposed a **17x ROI retention strategy**

### 💻 Technical Impact:
- Strong SQL analytics, segmentation, and business storytelling

---

## 🛠️ Tech Stack
- SQL Server  
- GitHub  

---

## 👤 Author
**Yakubu Hamza Ugbedeojo**  

📧 mailx0hamza@gmail.com  
