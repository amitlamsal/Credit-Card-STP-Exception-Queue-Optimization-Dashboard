# Credit Card STP & Exception Queue Optimization Dashboard
### End-to-End Business Analytics Project | Banking & Finance Domain | U.S. Credit Card Operations

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat&logo=mysql&logoColor=white)
![Excel](https://img.shields.io/badge/Excel-217346?style=flat&logo=microsoftexcel&logoColor=white)
![Status](https://img.shields.io/badge/Status-Complete-1D9E75?style=flat)

---

## Project Overview

This project mirrors a real Business Analytics engagement at a U.S. bank. A credit card operations division had no real-time visibility into its application processing performance — SLA breaches were discovered after the fact, exception queues were unmanaged, and there was no data-driven basis for improving automation efficiency.

The project delivers a complete solution: from Business Requirements Document through data generation, cleaning, EDA, Power BI dashboard build, UAT testing, key findings and actionable recommendations.

---

## The Business Problem

A U.S. bank processing credit card applications had:

- No real-time dashboard showing STP rate, manual review rate or SLA compliance
- SLA breaches discovered after they occur — no proactive alerting system
- Exception queue managed on FIFO basis with no aging or priority visibility
- No data on which exception types drive the most manual reviews
- STP rate of **46.7%** against an **80% policy target** — 33 percentage points below target

---

## Key Results

| KPI | Value | Benchmark | Status |
|---|---|---|---|
| Total Applications | 5,000 | Full year 2024 | ℹ️ |
| Approval Rate | 56.3% | 45–65% | ✅ On Target |
| STP Rate | 46.7% | ≥ 80% | ❌ Critical |
| Manual Review Rate | 53.3% | < 20% | ❌ Critical |
| SLA Breach Rate | 6.5% | < 5% | ⚠️ Amber |
| Default Rate | 4.3% | 3–5% | ✅ On Target |
| Avg Credit Score | 668 | 650–719 | ✅ Good Band |
| Avg Processing Time | 891 min | < SLA | ⚠️ Amber |

---

## Project Deliverables — 16 Professional Documents

| # | Deliverable | Phase | Format |
|---|---|---|---|
| 1 | Business Requirements Document (BRD) | Requirements | Word |
| 2 | Business Rules — 12 rules across 12 user stories | Requirements | Word |
| 3 | As-Is Process Flow Diagram | Process Design | Diagram |
| 4 | To-Be Process Flow Diagram | Process Design | Diagram |
| 5 | Data Dictionary — 18 columns, 10 DQ rules | Data Design | Excel |
| 6 | Synthetic Dataset — 5,000 records | Data | Excel |
| 7 | Data Cleaning & Validation Report | Data | Excel |
| 8 | Exploratory Data Analysis (EDA) Report | Data | Excel |
| 9 | Dashboard Wireframe — 3 pages | Design | Visual |
| 10 | Power BI Dashboard — 3 pages, 6 features | Build | Power BI |
| 11 | UAT Checklist — 25 test cases, 8 stakeholders | Testing | Excel |
| 12 | UAT Test Cases Document | Testing | Word |
| 13 | Key Findings Report — 8 findings | Analysis | Word |
| 14 | Recommendations Report — 6 recommendations | Analysis | Word |
| 15 | Executive Summary | Wrap-Up | Word |
| 16 | Presentation Deck — 16 slides | Wrap-Up | PowerPoint |

---

## Dashboard Pages

### Page 1 — Executive Overview
All 8 KPI tiles with RAG color coding, monthly application volume trend, STP vs Manual review trend, approval status breakdown, and product-level STP and SLA performance.

**Target users:** VP of Operations, Executive Leadership

### Page 2 — Operations Dashboard
STP vs Manual by channel, exception reason breakdown, queue aging bucket cards (Fresh/Aging/At Risk/Critical), bottleneck table with priority conditional formatting, SLA breach trend line, and processing time comparison.

**Target users:** Operations Manager, Process Improvement Analysts

### Page 3 — Risk Dashboard
Credit score band distribution with manual review trigger zone, approval rate by credit score band, DTI band distribution, high risk vs standard applicants donut, and SLA breach count by credit score band.

**Target users:** Credit Risk Manager, Credit Analysts

---

## Key Findings

| # | Finding | Severity |
|---|---|---|
| F-01 | STP rate of 46.7% is critically below the 80% policy target | 🔴 Critical |
| F-02 | Borderline Credit Score band is the primary driver of manual review | 🔴 Critical |
| F-03 | SLA breach rate of 6.5% is in the amber warning zone | 🟡 High |
| F-04 | Manual review applications take 55x longer than STP (1,659 vs 16 min) | 🟡 High |
| F-05 | 97% of pending queue is in the Critical aging bucket (7+ days) | 🟡 High |
| F-06 | Default rate of 4.3% is within the 3–5% industry benchmark | 🔵 Medium |
| F-07 | Good credit score band drives highest volume and most exceptions | 🔵 Medium |
| F-08 | Online channel drives 60% of volume with room for STP optimization | 🔵 Medium |

---

## Recommendations

| # | Recommendation | Priority | Timeline | Expected Impact |
|---|---|---|---|---|
| R-01 | Narrow credit score trigger band from 650–720 to 670–710 | 🔴 Critical | 0–3 months | STP +8–13pp |
| R-02 | Introduce secondary auto-decisioning for Good band applicants | 🔴 Critical | 3–6 months | STP +15–20pp |
| R-03 | Implement real-time SLA alerting and queue priority management | 🟡 High | 0–1 month | SLA breach -1.5pp |
| R-04 | Invest in automation programme to reduce manual review to <20% | 🟡 High | 6–12 months | STP ≥ 80% |
| R-05 | Online channel STP optimization leveraging digital data quality | 🔵 Medium | 3–6 months | Online STP +15pp |
| R-06 | Establish monthly KPI performance review using dashboard | 🔵 Medium | 0–1 month | Governance |

---

## Tools & Technologies

| Tool | Purpose |
|---|---|
| **Power BI** | Dashboard development — DAX measures, Power Query, 3-page interactive dashboard |
| **Python** | Synthetic data generation, data cleaning, EDA visualization |
| **SQL** | Data cleaning scripts — UPDATE, COUNTIFS, cross-field validation |
| **Power Query (M)** | Data transformation and cleaning in Excel/Power BI |
| **Excel** | EDA analysis, Data Dictionary, UAT Checklist |
| **Word** | BRD, Business Rules, Findings, Recommendations, Executive Summary |
| **PowerPoint** | 16-slide project presentation deck |
---

## Project Structure

```
credit-card-stp-exception-queue-dashboard/
│
├── 01_Requirements/
│   ├── Business_Requirements_Document.docx
│   └── Business_Rules_Document.docx
│
├── 02_Process_Design/
│   ├── As_Is_Process_Flow.png
│   └── To_Be_Process_Flow.png
│
├── 03_Data_Design/
│   ├── Data_Dictionary.xlsx
│   └── Data_Quality_Rules.xlsx
│
├── 04_Data/
│   ├── Credit_Card_Dataset.xlsx
│   ├── Credit_Card_Dataset_Cleaned.xlsx
│   └── Data_Cleaning_Validation_Report.xlsx
│
├── 05_EDA/
│   ├── EDA_Report.xlsx
│   └── eda_analysis.py
│
├── 06_Dashboard/
│   ├── Dashboard_Wireframe.png
│   └── Credit_Card_Dashboard.pbix
│
├── 07_UAT/
│   ├── UAT_Checklist.xlsx
│   └── UAT_Test_Cases.docx
│
├── 08_Analysis/
│   ├── Key_Findings_and_Insights.docx
│   └── Recommendations_Report.docx
│
└── 09_Presentation/
    ├── Executive_Summary.docx
    └── Credit_Card_Analytics_Presentation.pptx
```

## BA Project Lifecycle Coverage

This project covers the complete Business Analyst project lifecycle:

- ✅ **Requirements Gathering** — BRD, User Stories, Acceptance Criteria
- ✅ **Business Rules Documentation** — 12 rules mapped to 12 user stories
- ✅ **Process Mapping** — As-Is and To-Be swimlane diagrams
- ✅ **Data Design** — Data Dictionary with DQ rules
- ✅ **Data Generation** — Synthetic data following real U.S. banking distributions
- ✅ **Data Cleaning** — Python, Power Query and SQL approaches documented
- ✅ **Exploratory Data Analysis** — 8 KPI analyses with charts
- ✅ **Dashboard Wireframing** — 3-page mockup before build
- ✅ **Dashboard Development** — Power BI with DAX, drill-down, cross-filtering
- ✅ **UAT Testing** — 25 test cases across 12 user stories
- ✅ **Findings & Recommendations** — 8 findings, 6 actionable recommendations
- ✅ **Executive Communication** — Summary and 16-slide presentation

---

## About the Author

**Amit Lamsal**
MS Business Analytics — Webster University, St. Louis MO

5 years banking experience — Credit Risk & Operations | Siddhartha Bank Limited

[![LinkedIn](https://img.shields.io/badge/LinkedIn-amitlamsal-0077B5?style=flat&logo=linkedin)](https://www.linkedin.com/in/amitlamsal)
[![Email](https://img.shields.io/badge/Email-amitlamsal72@gmail.com-D14836?style=flat&logo=gmail)](mailto:amitlamsal72@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-amitlamsal-181717?style=flat&logo=github)](https://github.com/amitlamsal)
