# Employee Attrition & HR Insights Dashboard

An interactive Tableau dashboard built to analyze employee attrition patterns across departments, demographics, and job roles — transforming raw HR data into a decision-support tool for retention strategy.

---

## What This Project Does

HR teams often have attrition data but lack a clear view of **where** attrition is concentrated, **who** is leaving, and **what factors** correlate with it. This dashboard answers those questions through visual exploration.

Built entirely in Tableau with SQL and Excel preprocessing, it provides:
- A real-time view of attrition KPIs across the organization
- Drill-down filters by department, age group, job role, gender, and tenure
- Story points that walk stakeholders through key findings with context
- Actionable retention insights backed by the data

---

## Live Dashboard

[View on Tableau Public →](https://public.tableau.com) *(replace with your actual link)*

---

## Key Metrics Tracked

| KPI | Description |
|---|---|
| Overall Attrition Rate | % of employees who left in the observation period |
| Department-wise Attrition | Which departments have the highest turnover |
| Attrition by Age Group | Younger employees vs tenured employees |
| Satisfaction Score Distribution | Job satisfaction, environment satisfaction, work-life balance |
| Tenure Distribution | How long leavers had been with the company |
| Attrition by Job Role | Which roles are hardest to retain |

---

## Tech Stack

| Tool | Purpose |
|---|---|
| Tableau Desktop / Public | Dashboard design and visualization |
| SQL | Data querying and aggregation |
| Excel | Data cleaning and preprocessing |
| CSV (IBM HR Dataset) | Source data |

---

## Project Structure

```
hr-attrition-dashboard/
│
├── data/
│   └── hr_attrition.csv             # Cleaned IBM HR dataset
│
├── preprocessing/
│   └── cleaning_steps.xlsx          # Excel preprocessing steps
│   └── queries.sql                  # SQL queries used for aggregation
│
├── dashboard/
│   └── HR_Attrition_Dashboard.twbx  # Packaged Tableau workbook
│
├── outputs/
│   └── dashboard_screenshot.png     # Static preview
│   └── retention_insights.md        # Written findings and recommendations
│
└── README.md
```

---

## Dashboard Features

### Overview Page
- Total headcount, total attrition count, attrition rate
- Month-by-month attrition trend line
- Department-wise attrition bar chart

### Demographic Breakdown
- Attrition heatmap by age group × job role
- Gender split across attrition vs active employees
- Marital status correlation with attrition

### Satisfaction Analysis
- Distribution of job satisfaction scores among leavers vs stayers
- Environment satisfaction vs attrition rate scatter
- Work-life balance score segmentation

### Story Points (Guided Narrative)
A sequence of guided slides walking a non-technical stakeholder through:
1. The scale of the attrition problem
2. Which departments need immediate attention
3. What the data suggests about root causes
4. Recommended interventions

---

## Key Findings

- **Sales department** had the highest attrition rate — concentrated among employees with under 2 years tenure
- **Employees aged 25–34** showed the steepest attrition curve, suggesting early-career dissatisfaction
- **Low job satisfaction scores (1–2)** correlated strongly with attrition — employees with score 1 were 3x more likely to leave
- **Overtime workers** had significantly higher attrition — a structural workload issue, not a compensation one
- **Monthly income below median** combined with low satisfaction was the strongest combined predictor of attrition

---

## Retention Recommendations (from the data)

1. Focus onboarding and 6-month check-ins on Sales — that's where early attrition concentrates
2. Reduce overtime dependency in high-attrition roles — burnout is a stronger driver than pay
3. Implement satisfaction surveys at month 12 and 24 — these are the peak attrition windows
4. Consider role-specific retention bonuses for Laboratory Technicians and Sales Executives — two roles with both high attrition and high replacement cost

---

## How to Open the Dashboard

**Option 1 — Tableau Public (no install needed)**
Visit the live link above.

**Option 2 — Tableau Desktop**
```bash
# Clone the repo
git clone https://github.com/govindsinghtanwar/hr-attrition-dashboard
cd hr-attrition-dashboard

# Open the packaged workbook
# Double-click dashboard/HR_Attrition_Dashboard.twbx
# Or open via Tableau Desktop > File > Open
```


---

## What I Learned

- How to structure a BI dashboard for a non-technical audience — the story matters as much as the data
- Using Tableau story points to build a guided narrative, not just a collection of charts
- The difference between vanity metrics (headcount) and actionable metrics (attrition by tenure segment)
- How preprocessing quality directly affects dashboard reliability — garbage in, garbage out
