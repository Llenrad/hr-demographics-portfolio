# HR Employee Distribution Report

This Power BI report analyzes a sample company's workforce composition, demographic breakdown, and headcount trends. It demonstrates proficiency in data cleaning, SQL transformation using MySQL, and interactive dashboard development for HR analytics.

---

## Table of Contents
1. [Data Cleaning & Preparation](#data-cleaning--preparation)
2. [Key Visuals & Insights](#key-visuals--insights)
3. [Visuals](#Visuals)
4. [Strategic Use Cases](#strategic-use-cases)
5. [PDF Export](#pdf-export)
6. [Tools Used](#tools-used)
7. [Disclaimer](#disclaimer)

---

## Data Cleaning & Preparation

The dataset underwent several preprocessing steps to ensure accuracy and usability:

### General Cleaning
- Removed rows with missing or invalid `hire_date` and `termdate`
- Filtered out employees under 18 years old (`age >= 18`)
- Standardized column names (e.g., `location_state`, `gender`, `department`)
- Converted `termdate` from text to proper `DATE` format
- Replaced `'0000-00-00'` and empty strings in `termdate` with `NULL`

### Date Logic
- Extracted `YEAR(hire_date)` and `YEAR(termdate)` for time-based analysis
- Calculated **net change** in headcount per year: `hires - terminations`
- Created **cumulative headcount** by tracking active employees year-over-year

### Derived Metrics
- `termination_rate` per department
- `average_length_of_employment` in years
- Gender and age group distributions
- Headquarters vs. Remote employee split

---

## Key Visuals & Insights

1. **Gender Distribution** – Male, Female, and Non-Conforming breakdown  
2. **Age Group Distribution** – Employees across age bands  
3. **Race Distribution** – Counts by race categories  
4. **Headquarters vs Remote** – HQ vs. remote employee comparison  
5. **Employees by State** – Geographic distribution  
6. **Change in Employees (2000–2020)** – Headcount trend over time  
7. **Average Length of Employment** – Tenure in years  
8. **Age Distribution by Gender** – Cross-tab of age and gender  
9. **Gender Distribution by Department** – Gender mix per department  
10. **Termination Rate by Department** – Exit rates across departments

---
## Visuals

<img width="1069" height="625" alt="Hr Photo 1" src="https://github.com/user-attachments/assets/9e5a716f-a776-4f2f-b2a2-f92017572211" />
<img width="1041" height="609" alt="Hr Photo 2" src="https://github.com/user-attachments/assets/a18a82c0-c3db-4c27-a9d1-0c04822b5684" />


---

## Strategic Use Cases

- Identify departments with high turnover  
- Track diversity and inclusion metrics  
- Support workforce planning and recruitment  
- Monitor long-term retention trends

---

## PDF Export

The full visual summary of this report is available as a downloadable PDF:

**[HR_EmployeeReport.pdf](./HR_EmployeeReport.pdf)**

---

## Tools Used

- **Power BI Desktop** – Dashboard creation  
- **MySQL** – Data extraction and transformation  
- **Excel** – Initial cleaning and validation

---

## Disclaimer

This report is for portfolio demonstration only. It is based on publicly available data and does not reflect any personal or company-specific records.

Special thanks to **Her Data** for the original concept and dataset used in this adaptation.
