# SUPPORT Study — Patient Outcomes Dashboard
### Advanced Excel Analytics Project

![Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![Power Query](https://img.shields.io/badge/Power_Query-217346?style=for-the-badge&logo=microsoft&logoColor=white)

---

## 📋 Project Overview
An advanced Microsoft Excel dashboard analysing clinical outcomes for 9,105 patients from the SUPPORT Study (Study to Understand Prognoses, Preferences, Outcomes and Risks of Treatment). The dashboard provides interactive analysis of patient mortality, hospital costs, survival estimates and clinical indicators across disease groups, demographics and comorbidity profiles.

---

## 📊 Dataset
| Detail | Information |
|---|---|
| Source | UCI Machine Learning Repository |
| Study | SUPPORT — Study to Understand Prognoses Preferences Outcomes and Risks of Treatment |
| Patients | 9,105 |
| Variables | 47 |
| Time Period | Data collected up to December 31, 1994 |

### Variable Categories
- **Patient Demographics** — age, sex, race, income, education
- **Disease Information** — disease group, disease class, comorbidities
- **Clinical Indicators** — blood pressure, heart rate, temperature, lab values
- **Survival Estimates** — model predictions and physician estimates
- **Outcome Variables** — hospital death, overall death, functional disability
- **Cost Variables** — hospital charges, total cost, micro cost

---

## 🗂️ Workbook Structure
| Sheet | Purpose |
|---|---|
| Raw Data | Original cleaned dataset loaded via Power Query |
| Calculations | 10 summary sections with advanced formulas |
| Pivot Analysis | 8+ Pivot Tables with Slicers for deep analysis |
| Chart Data | Summary tables feeding all 12 dashboard charts |
| Helper | Hidden sheet storing dropdown validation lists |
| Dashboard | Main interactive visual dashboard |

---

## ⚙️ Technical Features

### 🔵 Data Cleaning — Power Query
- Imported raw CSV using Power Query
- Handled missing values across 47 variables using clinically validated imputation values sourced from HBiostat Repository
- Standardised text categories using Trim, Clean and Lowercase transformations
- Set correct data types for all 47 columns
- Created reproducible cleaning pipeline that refreshes automatically

### 🔵 Named Ranges
- Created 47 Named Ranges using Excel Table structured references
- Ensures formulas are readable and maintainable
- Eliminates hardcoded cell references

### 🔵 Calculations Sheet
- 10 summary sections covering Patient Overview, Mortality Analysis, Cost Analysis, Clinical Indicators, Survival Estimates, Comorbidities, Disease Group Breakdown, Age Group Breakdown, Gender Breakdown and Race Breakdown
- Advanced formulas used: COUNTIF, COUNTIFS, AVERAGEIF, AVERAGEIFS, SUMIF, SUMIFS, IFERROR

### 🔵 Pivot Tables
- 12+ interconnected Pivot Tables covering Deaths by Disease Group, Costs by Disease Group, Deaths by Age Group, Survival Estimates, Demographics by Race, Income vs Costs, Comorbidities vs Outcomes, DNR Status, Diabetes and Dementia Overview, Cancer Status and Breakdown by Sex
- Slicers connected to all Pivot Tables
- Conditional Formatting applied to all tables

### 🔵 Charts — 12 Visualisations
| Chart | Type | Insight |
|---|---|---|
| 1 | Clustered Bar | Hospital Deaths by Disease Group |
| 2 | Clustered Column | Patient Distribution by Age Group |
| 3 | Pie Chart | Gender Distribution |
| 4 | Combo Chart | Patients vs Death Rate by Disease |
| 5 | Stacked Bar | Cancer Status Breakdown |
| 6 | Line Chart | Model vs Physician Survival Estimates |
| 7 | Doughnut | DNR Status Distribution |
| 8 | Scatter Plot | Severity Score vs Hospital Charges |
| 9 | Bar Chart | Cost Breakdown by Disease Group |
| 10 | Box and Whisker | Age Distribution by Disease Group |
| 11 | Treemap | Patient Volume Hierarchy |
| 12 | Histogram | Severity Score Distribution |

### 🔵 Dashboard
- 5 Dynamic KPI Cards — Total Patients, Hospital Death Rate, Average Hospital Charges, Average Severity Score, Average 6 Month Survival

### 🔵 Patient Lookup Tool
- XLOOKUP powered search by Patient ID
- Instantly retrieves 20 patient fields including demographics, disease information, clinical measurements, cost data, survival estimates and comorbidity status
- Conditional formatting highlights hospital deaths, high severity scores and low survival estimates
- Error handling for invalid Patient IDs

### 🔵 Conditional Formatting
- Color scales for mortality rates
- Data bars for patient counts
- Icon sets for severity indicators
- Custom formula based rules for health equity insights
- Traffic light system for DNR analysis

---

## 🔍 Key Clinical Insights

**1. Disease Mortality** — Coma patients have the highest hospital death rate at 61% which is 2.4x higher than the study average of 26%. Colon Cancer has the lowest at 6%.

**2. Cost Paradox** — Metastatic cancer patients have the lowest hospital charges at $23,128 despite being critically ill suggesting palliative care pathways reduce in-hospital costs vs active treatment at $72,063.

**3. Disease Burden** — ARF/MOSF w/Sepsis accounts for 38% of all hospital deaths despite representing only 33% of total patients.

**4. Comorbidity Impact** — Patients with 4+ comorbidities show 70% higher severity scores and 90% higher hospital charges vs patients with no comorbidities.

**5. Survival Prediction Gap** — Model survival estimates consistently differ from physician estimates suggesting systematic bias in clinical prognosis.

**6. Health Equity** — Significant variation in charges and death rates across race and income groups highlights health equity disparities in critical care.

---

## 📈 Advanced Excel Skills Demonstrated
| Skill | Application |
|---|---|
| Power Query | Data import, cleaning, transformation |
| Named Ranges | 47 structured table references |
| XLOOKUP | Patient lookup tool |
| COUNTIFS | Multi-condition patient counting |
| AVERAGEIFS | Conditional clinical averages |
| SUMIFS | Conditional cost totals |
| IFERROR | Error handling throughout |
| Array Formulas | PERCENTILE IF for quartile analysis |
| Pivot Tables | 12+ summary tables |
| Slicers | Multi-table filtering |
| Data Validation | Dropdown filters and input control |
| Conditional Formatting | 20+ rules across all tables |
| Advanced Charts | Box and Whisker, Treemap, Scatter, Histogram |
| Cell Protection | Workbook security and locking |

---

## 🚀 How to Use

**Prerequisites** — Microsoft Excel 365 required for XLOOKUP and dynamic arrays

**Getting Started**
1. Download the Excel file
2. Enable editing if prompted
3. Go to Dashboard sheet
4. Use dropdown filters to explore data
5. Type any Patient ID between 1 and 9105 in the yellow search box
6. Use Pivot Analysis sheet for deeper exploration

**Refreshing Data**
1. Go to Data tab
2. Click Refresh All
3. All calculations and charts update instantly



## 📚 Data Source
Dataset: SUPPORT2 Clinical Study Dataset — UCI Machine Learning Repository
Imputation Values: HBiostat Repository, Professor Frank Harrell, Vanderbilt University
Citation: Knaus et al. (1995). The SUPPORT Prognostic Model. Annals of Internal Medicine.

---

## 👤 Author

- LinkedIn: https://www.linkedin.com/in/sindhoori-vadde-aa9b1a294/
- GitHub: https://github.com/Sindhu-Vadde/Excel-Projects  


---

## 📄 License
This project is for educational and portfolio purposes only. Dataset used under UCI ML Repository terms of use.

---

## 🔄 Project Status
✅ Power Query Data Cleaning
✅ Calculations Sheet
✅ Pivot Tables and Slicers
✅ Conditional Formatting
✅ 12 Dashboard Charts
✅ 5 KPI Cards
✅ Interactive Filters
✅ XLOOKUP Patient Lookup Tool
✅ Key Insights Panel
✅ Cell Level Protection
