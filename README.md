# 🏥 Hospital Emergency Room Dashboard

## 🔹 Project Overview

This **Hospital Emergency Room Dashboard** is a Power BI solution designed to visualize and analyze patient flow, satisfaction, department referrals, and admission patterns.  
The data covers **9,216 patient visits over a period of 19 months (April 2023 - October 2024)**.  
The main objective of this project is to help the hospital **optimize resources, reduce waiting times, and improve patient care delivery**.

---

## 🛠 Tools & Techniques

- **Excel:** For initial data cleaning and data validation.
- **Power Query:** To clean & transform raw data and to create interactive reports and visualizations.

---

## 🧮 Measures (DAX)

Below are key measures used in this Power BI Dashboard:

| **Measure / KPIs** | **DAX Formulas** |
|------------|------------|
| **No of Patients** | `DISTINCTCOUNT('Hospital ER_Data'[Patient Id])` |
| **Avg Wait Time1** | `FORMAT(AVERAGE('Hospital ER_Data'[Patient Waittime]), "0.0") & " " & "Min"` |
| **Satisfaction Score** | `AVERAGE('Hospital ER_Data'[Patient Satisfaction Score])` |
| **No of Patients Referred** | `CALCULATE(COUNTROWS('Hospital ER_Data'), 'Hospital ER_Data'[Department Referral] <> "None")` |

---

## 📐 Important KPIs & Metrics

- **Average Wait Time:** 35.3 minutes
- **Satisfaction Score:** 4.99/10
- **Admission Rate:** 50%
- **Most Referred Departments:** General Practice (1840), Orthopedics (995), Physiotherapy (276), Cardiology (248)

---

## 👥 Demographic and Behavioral Insights

- **Patient Age:** Large groups were adults 30-39 (about 1,200) and young adults 20-29 (about 1,188).
- **Race Distribution:** White (2,571), Black or African American (1,951), Multiracial (1,557), and Asian (1,060).
- **Admission vs Discharge:** Approximately 50% were discharged and 50% were admitted.

---

## ⏱ Peak Period Analysis

- **Busiest Days:** Monday (1,377), Saturday (1,322), Tuesday (1,318).
- **Busiest Hours:** 11 AM, 7 PM, 11 PM — reflecting a need for appropriate staffing during these periods.

---

## 🔹 Recommendations

✅ **Reduce Waiting Times:**  
Implement fast-track services for less severe cases and leverage technology to streamline patient flow.

✅ **Improve Late-Night Services:**  
Staff adequately during 11 pm to 6 am, maintain service cleanliness, and provide specialized care.

✅ **Target Department-Specific Improvement:**  
For male patients in Renal and for female patients in Physiotherapy, consider patient feedback to enhance service delivery.

---

## 📁 Summary

This Power BI Dashboard converts raw hospital data into actionable insight, helping stakeholders to:

- Allocate resources more efficiently.
- Reduce patient waiting time.
- Improve patient satisfaction and care delivery.

---



