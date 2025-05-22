# Project Overview
This Power BI project provides a comprehensive analysis of emergency room visit data to evaluate average wait times, monthly patient visits, referral patterns, patient satisfaction, and demographics. It helps healthcare administrators identify patterns, improve service delivery, and enhance patient experience.
## Data Files
-<a href="https://github.com/Thirisha255/Patients-Emergency-Room-Visit-Report-Power-BI-Project/blob/main/Hospital%20ER%20(1).csv">Dataset<a/>
##  Tools Used
- Power BI Desktop
- Power Query Editor
- DAX
- Star Schema Modeling
##  Data Cleaning Process
- Extracted AM/PM from the original timestamp field
- Merged First Name and Last Name into a new Full Name column using a space delimiter
- Created calculated columns and custom measures for improved insight
**Created a Date Table with the following columns:**
Date
Year
Month
Week Type (Weekday/Weekend)
Weekday
##  Key KPIs and Measures
- Total Patients: 4,632
- % Administrative Appointments: 49.35%
- % Non-Administrative Appointments: 50.65%
- Average Satisfaction Score: 5.45
- % Not Rated: 75.71%
- Average Wait Time: 35.53 minutes
- % Referred Patients: 41.15%
- % Walk-In Patients: 58.85%
**Gender Breakdown:**
- Male: 51.5%
- Female: 48.2%
- Unknown: 0.3%
**Age Group Buckets (via Age Classification Logic)**
Infancy: Age ≤ 2
Early Childhood: Age ≤ 6
Middle Childhood: Age ≤ 12
Teenager: Age ≤ 18
Adult: Age > 18
## Data Modeling
Built a Star Schema
Fact Table: Patient Visit Table
Dimension Tables: Date, Department, Age Group
One-to-Many Relationships used between Date and Fact Table
## 📈 Visualizations Created
Total Patient Visits by Year and Month (line chart with min/max markers)
🔴 Minimum Point (Jan): 212 visits
🟢 Maximum Point (May): 540 visits
Total Patients by Age Group (Bar Chart)
Adults had the highest number of visits: 3,550
Visits by Week Type
Total Visits by Department Referral
Top Referrals: General Practice (2,726), Orthopedics (924)
Heatmap Matrix for Avg Satisfaction & Wait Time
Rows: Patient Race
Columns: Age Groups
Values: Average Satisfaction / Wait Time
Dynamic Caption (Measure: Hit Map Caption):
If Average Wait Time selected → “The darkest green on the scale denotes low wait time”
If Average Satisfaction is selected → “Patients are most satisfied when the scale shows the darkest green”
## Dashboard
-<a href="https://github.com/Thirisha255/Patients-Emergency-Room-Visit-Report-Power-BI-Project/blob/main/patient%20report.png">Dashboard image<a/>
##  Key Insights
- Most visits occur on weekdays (71.2%)
- Adults are the most frequent emergency room visitors
- The majority of visits are non-referred (walk-in)
- Satisfaction and wait time vary significantly by race and age group
- High satisfaction is often linked to shorter wait times and specific age brackets
