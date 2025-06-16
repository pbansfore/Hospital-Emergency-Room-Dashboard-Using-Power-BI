# 🏥 Hospital Emergency Room Dashboard

## 🔹 Project Overview

This **Hospital Emergency Room Dashboard** is a Power BI solution designed to visualize and analyze patient flow, satisfaction, department referrals, and admission patterns.  

The data covers **9,216 patient visits over a period of 19 months (April 2023 - October 2024)**.  
The main objective of this project is to help the hospital **optimize resources, reduce waiting times, and improve patient care delivery**.

---

## 🛠 Tools & Techniques

- **Excel:** For initial data cleaning and data validation.
- **Power BI:** To clean & transform raw data and to create interactive reports and visualizations.

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

## 🔍 Findings

➥ **Patient Flow and Volume:**  
- The department treated **9,216 unique patients** over 19 months (April 2023–October 2024).
- **Busiest days:** Saturdays (1,377) & Sundays (1,318).
- **Busiest hours:** 10 PM to 12 AM & 06 AM to 08 AM, indicating a need for appropriate staffing during these periods.

➥ **Patient Demographics:**  
- Large age groups were **adults 30–39 (about 1,200)** and **young adults 20–29 (about 1,188)**.
- The racial distribution highlights **White (2.6k)**, **Black or African American (2.0k)**, **Multiracial (1.6k)**, and **Asian (1.1k) patients**.

➥ **Admission and Referral Trends:**  
- **About 50% were discharged and 50% were admitted.**
- The most frequently referred department was **General Practice (1.8k)**, followed by **Orthopedics (1.0k)**, **Physiotherapy (0.3k)**, and **Cardiology (0.2k)**.
- Large number (about 5,400) required no department referrals.

➥ **Patient Experience:**  
- The average waiting time was **35.3 minutes** — fairly lengthy for an Emergency Department.
- The average satisfaction score was **4.99/10**, reflecting a need for service improvement.

---

## 🚀 Recommendations

✅ **Reduce Waiting Times:**  
- Implement **fast-track services for less severe cases**.
- Leverage **technology to streamline patient flow** and reduce bottlenecks.

✅ **Improve Late-Night and Early-Morning Services:**  
- Allocate additional staffing during **10 pm to 8 am**.
- Provide specialized care and a comfortable, well-equipped environment during overnight hours.

✅ **General Recommendations:**  
- Monitor busy periods closely to align staffing with patient flow.
- Develop initiatives to **improve patient satisfaction**, from reducing waiting time to improving communication and care delivery.

---

## 📁 Summary

Using these insights, the hospital can **improve patient satisfaction and care delivery by reducing waiting periods, optimizing staffing during peak hours, and addressing department-specific weaknesses**. Implementing these recommendations will help align service delivery with patient needs and drive **higher health outcomes in the Emergency Department**, ultimately strengthening the hospital’s ability to provide **timely, efficient, and patient-centric care**.


---




