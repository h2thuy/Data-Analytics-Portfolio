#  Developer Salary Analysis - Stack Overflow Survey

This project explores global developer salaries using data from the Stack Overflow Developer Survey. It focuses on how salaries vary by country and job role, providing insights for both developers and employers.

---

##  Overview

The main objectives of this project are to:

- Identify countries with the highest average developer salaries
- Discover which developer roles are the best-paid
- Understand salary distribution across various regions and job types

---

##  Dataset

- **Source:** Stack Overflow Developer Survey
- **Size:** ~70,000 responses
- **Relevant fields:**
  - `Country`
  - `ConvertedCompYearly` (Annual compensation in USD)
  - `DevType` (Developer roles)
  - `EdLevel` (Education level)
  - `YearsCodePro` (Years of professional experience)

---

##  Tools & Technologies

- **Programming Language:** Python
- **Libraries:**  
  - `pandas` for data manipulation  
  - `numpy` for numerical operations  
  - `matplotlib` & `seaborn` for data visualization  
  - `scikit-learn` (reserved for potential ML tasks)

---

##  Data Cleaning

- Removed duplicates and null values in critical columns
- Filtered unrealistic salary values (< $1,000 or > $500,000)
- Split multi-role values from `DevType` using `;`
- Normalized and transformed data types for analysis

---

##  Exploratory Analysis

###  Salary by Country

- Grouped by `Country`
- Filtered to include only countries with ≥ 100 responses
- Calculated and visualized average salaries
- Top countries: USA, Switzerland, Israel

###  Salary by Developer Role

- Used `explode()` to handle multiple roles per individual
- Filtered for roles with ≥ 100 responses
- Calculated average salaries
- Top roles: Engineering Manager, Data Scientist, Cloud Engineer

---

##  Key Insights

- Developer salaries are highest in North America and Western Europe.
- Management and data-related roles tend to earn more.
- Clear evidence that specialization and leadership drive salary increases.

---
