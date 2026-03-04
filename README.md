# 📊 Palmoria Group — HR Gender Equity & Compensation Analysis

> **"Now, the future of gender equality in Palmoria lies in your hands."**  
> — Mr. Yunus Shofoluwe, CHRO, Palmora Group

---

## 🗂 Project Overview

This project delivers a full end-to-end **HR Analytics case study** for **Palmoria Group**, a Nigerian manufacturing company operating across **Lagos, Abuja, and Kaduna**. Following media coverage highlighting gender inequality within the organisation, the executive team commissioned a data-driven investigation to identify disparities in gender representation, compensation, performance ratings, and regulatory compliance.

The analysis was built using **Power BI** and covers a workforce of **946 employees** across **12 departments**.

---

## 🔍 Business Problem

Palmoria Group was publicly criticised under the headline:

> *"Palmoria, the Manufacturing Patriarchy"*

The CEO, **Mr. Ayodeji Chukwuma**, and CHRO, **Mr. Yunus Shofoluwe**, needed actionable insights to address:

- Gender representation gaps across regions and departments
- Whether a gender pay gap exists — and where
- Compliance with a new **$90,000 minimum salary** regulation
- Equitable performance rating practices
- Fair and transparent bonus allocation

---

## 📁 Repository Structure

```
palmora-hr-analysis/
│
├── 📊 Palmoria_Group_Analysis.pbix       # Power BI dashboard file
├── 📄 Palmoria_Stakeholder_Report.docx   # Executive stakeholder report
├── 📁 data/
│   ├── hr_data.csv                      # Cleaned employee dataset
│   └── bonus_rules.csv                  # Bonus allocation rules by rating
├── 📁 screenshots/
│   ├── dashboard_overview.png
│   ├── gender_ratings.png
│   └── salary_compliance.png
└── README.md
```

---

## 🛠 Tools & Technologies

| Tool | Purpose |
|------|---------|
| **Power BI** | Data modelling, DAX measures, interactive dashboards |
| **Microsoft Excel** | Data cleaning & pre-processing |
| **DAX** | Custom measures for salary bands, bonus calculations, gender splits |
| **Power Query** | ETL — removing nulls, reassigning undisclosed gender, filtering inactive employees |

---

## 🧹 Data Cleaning Steps

Before analysis, the following transformations were applied:

1. **Employees with no salary** (no longer with the company) → **Removed**
2. **Employees with NULL department** → **Removed**
3. **Employees with undisclosed gender** → **Reassigned as "Others"** (generic gender status)

---

## 📈 Dashboard Pages

### Page 1 — Salary & Compensation Overview
![Dashboard Overview](screenshots/dashboard_overview.png)
<img width="472" height="260" alt="Screenshot 2026-03-04 115440" src="https://github.com/user-attachments/assets/1b580f04-322a-4b48-b397-5df5d96dee67" />

Key metrics displayed:
- **$69.72M** total salary bill
- **$71.92M** total pay (salary + bonus)
- **$2.20M** total bonus allocated
- **3** regions operational
- Salary band distribution by location and gender
- Department-level pay comparison

---

### Page 2 — Gender & Workforce Distribution
![Gender Ratings](screenshots/gender_ratings.png)
<img width="471" height="266" alt="Screenshot 2026-03-04 115408" src="https://github.com/user-attachments/assets/9fae8e15-b937-4562-becb-270fa76da80b" />

Key metrics displayed:
- **946** total active employees
- Gender split: **49.2% Male | 46.6% Female | 4.2% Others**
- Count of gender by department (12 departments)
- Performance rating distribution by gender
- Gender breakdown across all 3 locations

---

### Page 3 — Performance Ratings & Bonus Analysis
![Salary Compliance](screenshots/salary_compliance.png)
<img width="466" height="257" alt="Screenshot 2026-03-04 115314" src="https://github.com/user-attachments/assets/de22be0b-3198-4920-9172-777ff6e82600" />

Key metrics displayed:
- Count of ratings per department, by gender
- Bonus allocation by department and gender
- **12** departments tracked
- Rating categories: Very Good · Good · Average · Poor · Very Poor · Not Rated

---

## 🔑 Key Findings

### 1. Gender Distribution
| Gender | Count | % of Workforce |
|--------|-------|----------------|
| Male | 465 | 49.2% |
| Female | 441 | 46.6% |
| Others | 40 | 4.2% |
| **Total** | **946** | **100%** |

> The workforce is broadly balanced at an organisation level. However, technical departments (Engineering, R&D) show a slight male skew — a structural pattern common in manufacturing.

---

### 2. Performance Ratings by Gender
| Rating | Female | Male | Others | Total |
|--------|--------|------|--------|-------|
| Average | 190 | 212 | 18 | 420 |
| Good | 89 | 82 | 9 | 180 |
| Poor | 58 | 70 | 3 | 131 |
| Very Good | 49 | 41 | — | 90 |
| Not Rated | ~35 | ~32 | ~4 | 71 |
| Very Poor | ~20 | ~30 | ~4 | 54 |

> ⚠️ **71 employees are unrated** — these employees cannot be fairly rewarded or developed without a formal review.

---

### 3. Gender Pay Gap
| Gender | Total Pay | % Share |
|--------|-----------|---------|
| Male | $36M | 50.1% |
| Female | $33M | 45.8% |
| Others | $3M | 4.1% |

> While the top-line figures reflect headcount differences, a **role-matched pay audit** is recommended for Engineering, Sales, and R&D — where structural gaps are most likely to exist.

---

### 4. Salary by Region
| Region | Total Payroll | % Share |
|--------|--------------|---------|
| Lagos | $26.65M | 38.2% |
| Kaduna | $24.12M | 34.6% |
| Abuja | $18.95M | 27.2% |

---

### 5. ⚠️ Regulatory Compliance — $90,000 Minimum Salary

> A new government regulation requires all manufacturing companies to pay a **minimum of $90,000** per annum.

| Salary Band | Employees | Status |
|-------------|-----------|--------|
| $100,000+ | 202 | ✅ Compliant |
| $90,000–$100,000 | 108 | ✅ Compliant |
| $80,000–$90,000 | 105 | ❌ Below minimum |
| $70,000–$80,000 | 117 | ❌ Below minimum |
| $60,000–$70,000 | 99 | ❌ Below minimum |
| $50,000–$60,000 | 96 | ❌ Below minimum |
| $40,000–$50,000 | 118 | ❌ Below minimum |
| $30,000–$40,000 | 101 | ❌ Below minimum |

> **~67% of employees (~636 out of 946) fall below the $90,000 regulatory minimum.**  
> This is Palmora's most urgent compliance and legal risk.

---

### 6. Bonus Allocation
| Region | Estimated Bonus | % of Total |
|--------|----------------|------------|
| Lagos | ~$840K | ~38% |
| Kaduna | ~$760K | ~35% |
| Abuja | ~$600K | ~27% |
| **Total** | **$2.20M** | **100%** |

> Bonuses are rating-driven. Since females proportionally earn more "Good" and "Very Good" ratings, they are well-positioned under the current bonus model — but the distribution should be monitored annually.

---

## ✅ Recommendations

| Priority | Action | Timeline |
|----------|--------|----------|
| 🔴 **URGENT** | Develop a phased salary uplift plan to bring all employees to $90,000+ | Immediate |
| 🟠 **HIGH** | Commission a role-matched pay equity audit in Engineering, Sales & R&D | Within 30 days |
| 🟡 **MEDIUM** | Complete performance reviews for all 71 unrated employees | Within 90 days |
| 🟢 **MONITOR** | Establish a bi-annual Gender Equity Scorecard across all departments | Ongoing |

---

## 📄 Deliverables

- [x] Power BI Dashboard (3 pages)
- [x] Executive Stakeholder Report (Word Document)
- [x] Salary compliance analysis
- [x] Bonus allocation by employee, department, and region
- [x] Gender distribution analysis
- [x] Performance rating breakdown by gender

---

## 👤 Author

**HR Analytics Consultant**  
*Commissioned by Palmora Group CHRO — Mr. Yunus Shofoluwe*  
*March 2026*

---

## 📜 Disclaimer

> This analysis was conducted using internal Palmora Group HR data provided for the purpose of this engagement. All findings are confidential and intended solely for executive leadership review. No personal employee data is published in this repository.

---

*⭐ If this project was helpful, consider starring the repository!*

