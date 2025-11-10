# 🎓 Student Marksheet Data Visualization Dashboard
---
**Project Title:** Student Marksheet Data Visualization  
**Tools Used:** Microsoft Power BI, Power Query, DAX, Excel 

----

## 📘 Project Overview
This project presents an **interactive Power BI dashboard** for analyzing student marks and academic performance across multiple subjects and semesters.  
It enables users to gain insights into student performance trends, subject-wise comparisons, and overall grade distribution.

The goal of this project is to **automate data analysis** for student marksheets, helping teachers, institutions, or administrators easily evaluate student progress through visual insights.

---

## 🎯 Objectives
- Visualize student marks data from Excel or CSV using **Microsoft Power BI**  
- Identify **top-performing students, weak subjects**, and **class average trends**  
- Automate data refresh and transformations using **Power Query**  
- Build custom metrics using **DAX formulas** for grading and pass percentage  

---

## 📊 Key Insights & Features
- **Student Performance Overview:** Displays total marks, average marks, and overall pass percentage  
- **Subject Analysis:** Compare performance across subjects with bar and line charts  
- **Top 10 Students:** Highlights highest-performing students with dynamic filtering  
- **Grade Distribution:** Visualizes count of students in each grade (A, B, C, D, F)  
- **Gender-wise & Semester-wise Comparison:** Provides insights into academic performance trends  

---

## 🧠 DAX Measures Used
```dax
Total Marks = SUM(Marks[Total])
Average Marks = AVERAGE(Marks[Total])
Pass % = DIVIDE(CALCULATE(COUNTROWS(Marks), Marks[Result] = "Pass"), COUNTROWS(Marks)) * 100
