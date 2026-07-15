# Digital Workplace Adoption Dashboard 📊

**Tools:** Python | Power BI | DAX  
**Industry:** Enterprise Technology / Digital Workplace

## Overview
Simulated a digital workplace analytics environment tracking tool adoption, 
engagement, and retention risk across 300 colleagues and 2,000 usage events 
over a 6-month period. Built a Python data pipeline to generate realistic 
behavioral data, then delivered a 2-page Power BI executive scorecard 
measuring adoption trends, feature utilization, and at-risk user identification 
across 7 departments.

## Dashboard Preview

![Executive Overview]()

## Key Findings
- **68% average adoption rate** — 32% of colleagues never logged in
- **97 High Risk users** — one third of the workforce is disengaged
- **Technology leads engagement** (0.64 score, 28.6 min avg session) vs 
  Legal (0.29 score, 13.7 min) — nearly 2x gap
- **Analytics Portal is the most adopted feature** — 219 unique users
- **Adoption trending upward** — 68.3% in January to 69.7% in June

## Dashboard Pages

### Page 1 — Executive Overview
- 6 KPI cards: Total Colleagues, Active Users, Adoption Rate, Avg Session Duration, High Risk Users, Engaged Users
- Monthly Adoption Rate trend line chart
- Engagement Score by Department bar chart
- Feature Adoption by Unique Users bar chart
- User Risk Distribution donut chart (Engaged / Medium Risk / High Risk)
- Department and tool slicers

### Page 2 — Department Deep Dive
- Session Duration by Department bar chart
- Tool Adoption by Unique Users bar chart
- User Risk Detail table (role, risk flag, sessions, engagement score)
- Department slicer for filtered analysis

## Data Pipeline
Built entirely in Python using pandas and NumPy:

| File | Description |
|---|---|
| adoption_users.csv | 300 colleagues with department, role, tenure, engagement score |
| adoption_events.csv | 2,000 usage events with tool, feature, session duration, actions |
| adoption_features.csv | Feature adoption summary — unique users and avg session metrics |
| adoption_tools.csv | Tool adoption summary — sessions and unique users per tool |
| adoption_dept_scorecard.csv | Department-level scorecard with engagement and adoption rates |
| adoption_user_summary.csv | Per-user summary with risk flag classification |
| adoption_mau.csv | Monthly active users and adoption rate over 6 months |
| adoption_monthly_trend.csv | Monthly sessions, actions, duration, and adoption rate trends |

## DAX Measures
- `Total Users` — COUNTROWS of users table
- `Active Users` — distinct user count from events
- `Overall Adoption Rate` — active / total formatted as %
- `Avg Session Duration` — average session length in minutes
- `High Risk Users` — FILTER count where risk_flag = High Risk
- `Engaged Users` — FILTER count where risk_flag = Engaged

## Skills Demonstrated
Python · pandas · NumPy · Power BI · DAX · Executive Reporting ·
Adoption Analytics · KPI Scorecard Design · Risk Segmentation

## Live Portfolio
