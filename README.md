# 📊 Patient Record Analysis Dashboard (Excel)

## Project Overview
This project features a comprehensive end-to-end business dashboard developed in Excel. The dashboard tracks key performance indicators (KPIs) such as the number of patients, average patient wait time, average patient satisfaction score, and other patient-related information over two years.

---

## 🎯 Business Objective
- Number of Patients:- Count the total number of patients visiting the ER each day. Show a daily trend with an area sparkline to spot patterns like busy days or seasonal trends.
- Average Wait Time:- Find the average time patients wait to see a medical professional. Use an area sparkline to track daily changes and highlight days with longer wait times that might need improvements.
- Patient Satisfaction Score:- Check the average daily satisfaction score of patients to assess service quality. Use an area sparkline to show trends, spot drops in satisfaction, and link them to busy times or challenges.
- Charts to create:-
Patient Admission Status: Show how many patients were admitted vs. not admitted.
Patient Age Distribution: Group patients by age.
Timeliness: Measure the percentage of patients seen within 30 minutes.
Gender Analysis: Display the number of patients by gender. 
Department Referrals: Check which departments patients are referred to the most.

---

## 🛠 Tools & Technologies
- Excel
- DAX (Data Analysis Expressions)
- Data Cleaning & Transformation
- CSV Data Processing
- Data Modeling
- Data Visualization
- Power Query 
- Power Pivot

---

## 📂 Dataset Information
Dataset Used: AdventureWorks Dataset (Maven Analytics) 
Data Source: CSV files  

Data Include:
- Hospital Records Data 

---

## ⚙️ Data Preparation & Modeling
- Imported dataset using Power Query 
- Cleaned and transformed raw data using Power Query
- Handled missing and inconsistent values
- Created Calendar Table to create relationship of the calendar table with all the other tables that contains date using Power Query
- Data Modeling using Power Pivot
- Created Calculated Columns using DAX Calculations in Power Pivot
  -> DAX Formula for Age Group: =if([Patient Age]>=70,"70-80",if([Patient Age]>=60,"60-69",if([Patient Age]>=50,"50-59",if([Patient Age]>=40,"40-49",if([Patient Age]>=20,"20-39",if([Patient Age]>=10,"10-19","0-9"))))))
  -> DAX Formula for =IF([Patient Waittime]<30,"Within Time","Delay")
- Designed KPI metrics to show business performance 
- Presented the Total Customers by Country on Map (6 countries are USA,Canada,Australia, France, UK and Germany)

---

## 📊 Dashboard Features

### 🔹 Executive Dashboard
- No. of Patients, Average Patient Wait Time and Average Patient Satisfaction Score KPIs
- Patient Admission Status, to show how many patients were admitted within time or admitted after delay (expected time is of less than and equal to 30 minutes)
- Gender wise distribution of Patients through Donut Chart 
- No. of Patients that were referred by different departments displayed through line chart 
- Interactive slicer panel of months as well as year to filter the data acccording to user's needs 
- No. of Patients divided into different age group categories 

### 🔹 No. of Patient Monthly Analysis
- A detailed area plot illustrating the monthly number of patients treated each month over a span of two years

### 🔹 Patient Satisfaction Score 
- An area plot demonstrating average patient satisfaction score each month over a span of two years

### 🔹 Patient Wait Time
- An area plot demonstrating average wait time spend by patient in the hospital for each month over a span of two years

---

## 📈 Key Insights
- In June 2023, 
- No. of Patients is 506
- Avg. Wait Time of 35.58 Minutes 
- Avg. Patient Satisfaction Score of 5.18 
- The no of patients that were attended within time is 184 out of 506 patients (64%) and patient that were attended with delay is 36% of total 
- The age group having the most number of Patients is in the age group of (20-39)
- The top department from where the department referred is most is General Practice followed by Orthopedics.

---

## 🖼 Dashboard Screenshots
![Dashboard Preview](https://github.com/RaadheySharma/patient-record-analysis-dashboard-excel/blob/main/Main%20Dashboard.png)
![No of Patients](https://github.com/RaadheySharma/patient-record-analysis-dashboard-excel/blob/main/No%20of%20Patients.png)
![Avg Patient Satisfaction Score](https://github.com/RaadheySharma/patient-record-analysis-dashboard-excel/blob/main/Patient%20Wait%20Time.png)
![Avg Patient Wait Time](https://github.com/RaadheySharma/patient-record-analysis-dashboard-excel/blob/main/Patient%20Wait%20Time.png)

---
