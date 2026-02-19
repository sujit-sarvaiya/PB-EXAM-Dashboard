# 📊 Power BI Student Performance Dashboard

Link- https://app.powerbi.com/groups/me/reports/50240bd7-9784-4267-982f-f6ec6f804e0b/13d7bf13a99b9f0058a4?experience=power-bi

## 📌 Project Overview

This project is an interactive Student Performance Dashboard created
using Power BI.\
The dashboard analyzes student academic performance, attendance records,
and behavior data.

------------------------------------------------------------------------

## 📂 Datasets Used

1.  **Students.csv**
    -   StudentID, Name, Gender, Class, Section
2.  **Scores.csv**
    -   StudentID, Subject, ExamType, Score, MaxScore, Term
3.  **Attendance.csv**
    -   StudentID, Date, Status (Present/Absent), Reason
4.  **Behavior.csv**
    -   StudentID, Date, BehaviorType, Notes

------------------------------------------------------------------------

## 🔄 Data Modeling

-   Created relationships:
    -   Students\[StudentID\] → Scores\[StudentID\]
    -   Students\[StudentID\] → Attendance\[StudentID\]
    -   Students\[StudentID\] → Behavior\[StudentID\]
-   Relationship Type: One-to-Many (1:\*)
-   Students table used as Dimension table.

------------------------------------------------------------------------

## 🧮 DAX Measures Created

-   \% Score = DIVIDE(SUM(Score), SUM(MaxScore))
-   Average Score = AVERAGE(Score)
-   Attendance % = Present Count / Total Attendance
-   Behavior Count = COUNT(BehaviorType)
-   Performance Category (High / Medium / Low using SWITCH)
-   Total Students = DISTINCTCOUNT(StudentID)
-   Avg Attendance KPI
-   Avg % Score KPI

------------------------------------------------------------------------

## 📊 Visualizations

-   ✅ Card Visuals:
    -   Total Students
    -   Average Score
    -   Avg Attendance
-   📊 Bar Chart:
    -   Average Score by Subject and Class
-   📈 Line Chart:
    -   \% Score by Term (Performance Trend)
-   🍩 Donut Chart:
    -   Behavior Count by Behavior Type
-   📋 Table:
    -   Student-wise scores with % Score

------------------------------------------------------------------------

## 🎨 Conditional Formatting

Applied on % Score column: - ≥ 80% → Green - 40% -- 79% → Yellow - \<
40% → Red

------------------------------------------------------------------------

## 🎛 Interactivity

-   Slicers for Class, Section, Subject, and Term
-   Drillthrough page for Student Profile
-   Clean and professional dashboard layout

------------------------------------------------------------------------

## 📱 Optional Enhancement

-   Mobile layout optimized for Power BI mobile app

------------------------------------------------------------------------

## ✅ Final Outcome

A fully interactive Student Performance Dashboard including: - KPI
indicators - Academic performance trends - Attendance analysis -
Behavior tracking - Professional formatting and structured data modeling

------------------------------------------------------------------------

### 👨‍💻 Developed using:

Microsoft Power BI Desktop
