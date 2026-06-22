# 📊 Insurance Analytics Dashboard

> End-to-end insurance business analytics project covering SQL database design, Power BI dashboards, and Excel automation — built to track brokerage revenue, policy performance, sales pipeline, and team KPIs across 6 major Indian cities.

---

## 📌 Project Overview

This project analyses the complete operations of an insurance brokerage firm — from policy renewals and revenue tracking to sales opportunities and account executive performance. The data spans branches across **Ahmedabad, Mumbai, Delhi, Bengaluru, Chennai, Pune, and Hyderabad**.

### Business questions answered:
- Which branches and solution groups generate the most brokerage revenue?
- What is the renewal vs lapse rate across product groups?
- How are account executives performing against individual budgets?
- Which sales opportunities are in the pipeline and at what stage?
- How does invoice revenue trend across months and regions?

---

## 🗂 Project Structure

```
insurance-analytics-dashboard/
├── database/
│   └── insurance_analytics.sql       ← Full MySQL database dump (11 tables)
├── powerbi/
│   └── Insurance_Analytics_BI.pbix   ← Power BI dashboard file
├── excel/
│   └── Insurance_dashboard.xlsm      ← Excel dashboard with VBA macros
└── README.md
```

---

## 🗃 Database Schema

MySQL database with **11 tables** covering the full insurance business model:

| Table | Description |
|---|---|
| `brokerage` | Core revenue table — policy-level brokerage amounts, renewal status, lapse reasons |
| `invoice` | Invoice-level revenue by branch, solution group, and account executive |
| `opportunity` | Sales pipeline — premium amounts, revenue, deal stages, product groups |
| `individual_budgets` | Per-executive new business, cross-sell, and renewal budgets |
| `meeting` | Client meetings tracked by executive and branch |
| `dim_policy` | Policy dimension — policy details and attributes |
| `dim_client` | Client dimension — client profiles and types |
| `dim_account_exe` | Account executive dimension |
| `dim_branch` | Branch dimension — 7 city branches |
| `dim_solution_group` | 10 solution groups across Corporate, Commercial, SME segments |
| `fees` | Fee-based revenue transactions |

### Key solution groups tracked:
`Employee Benefits` · `Marine` · `Property/BI` · `Liability` · `Construction & Infrastructure` · `Trade Credit` · `SME` · `Emerging Corporates`

---

## 📊 Power BI Dashboard

**File:** `powerbi/Insurance_Analytics_BI.pbix`

Built using DAX measures and relationships across all 11 tables.

### Dashboard pages include:
- **Revenue Overview** — Total brokerage by branch, product group, and solution group
- **Policy Performance** — Active vs lapsed vs renewed policies with trend lines
- **Sales Pipeline** — Opportunity stages, premium amounts, and closing dates
- **Executive Scorecard** — Actual vs budget performance per account executive
- **Invoice Analysis** — Monthly invoice revenue by branch and income class
- **Meeting Activity** — Client engagement tracking by executive and region

### Key DAX measures used:
- `Total Brokerage Amount` — Sum of brokerage with renewal/lapse filters
- `Budget vs Actual Variance` — New business and renewal performance gaps
- `Renewal Rate %` — Policy renewal success rate by product group
- `Pipeline Value` — Total premium and revenue in active opportunity stages

---

## ⚙️ Excel Dashboard

**File:** `excel/Insurance_dashboard.xlsm`

Interactive Excel workbook with:
- **VBA Macros** for automated data refresh and report generation
- **Pivot Tables** summarising revenue by branch, executive, and product
- **Power Pivot** data model connecting multiple data sources
- **Conditional Formatting** for KPI traffic-light indicators
- **Slicers** for dynamic filtering by branch, date, and solution group

---

## 🛠 Tools & Technologies

| Layer | Tool | Purpose |
|---|---|---|
| Database | MySQL 8.0 | Data storage, schema design, querying |
| BI Dashboard | Power BI Desktop | Interactive visualisations, DAX measures |
| Reporting | Advanced Excel + VBA | Automated reporting, pivot analysis |
| Data Modelling | Power Pivot | Multi-table relationships in Excel |

---

## 🚀 How to Run

### SQL Database
1. Install MySQL 8.0+
2. Open MySQL Workbench or any MySQL client
3. Run: `source insurance_analytics.sql`
4. Database `insurance_analytics` will be created with all 11 tables and data

### Power BI Dashboard
1. Install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free)
2. Open `Insurance_Analytics_BI.pbix`
3. If prompted, update the data source connection to your MySQL instance
4. Click **Refresh** to load the latest data

### Excel Dashboard
1. Open `Insurance_dashboard.xlsm` in Microsoft Excel (2016 or later)
2. Enable Macros when prompted
3. Use the slicers and buttons to interact with the dashboard

---

## 🎓 Course & Certification

This project was developed as part of the:
- **Data Analyst Programme** — ExcelR, Bengaluru | Completed with Distinction *(May 2026)*

---

## 👤 Author

**Vinayak M**
- 📧 mvinayak96@gmail.com
- 💼 [LinkedIn](https://www.linkedin.com/in/vinayak-m-b78196ab)
- 🌐 [Portfolio](https://vinayakm.vercel.app)
