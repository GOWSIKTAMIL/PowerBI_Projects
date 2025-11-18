# Objective

The objective of this project is to analyze employee attrition within the organization using demographic data, job-related factors, departmental information, and satisfaction scores. This analysis helps identify why employees leave and supports strategic HR decision-making to improve retention and workforce stability.

# Project Highlights

This project focuses on important HR metrics such as:

Total employees vs employees who quit

Attrition percentage

Department-wise resignations

Gender-wise and age-band-wise attrition

Job satisfaction levels

Education field impact on attrition

Marital status and gender influence on employee count

These insights help the HR department understand which groups are more likely to quit and what factors contribute most to attrition.

# Dashboard Visualization
# DASHBOARD
<img width="1361" height="814" alt="image" src="https://github.com/user-attachments/assets/8960b330-51cc-40b9-a0a2-38783b11d592" />

The dashboard displays KPIs, charts, and comparison visuals to give a complete overview of employee attrition patterns across the organization.

# Dashboard Insights
1. KPI Summary

The KPI cards display:

Total Employees: 1470

Employees Quit: 237

Attrition Rate: 16%

Average Age: 36.92

Current Employees: 1233

Monthly Income: 10M

These KPIs help HR understand overall workforce trends instantly.

2. Employee Quit by Department

A pie chart represents the resignation distribution across departments:

R&D

Sales

HR

This shows which department has the highest attrition and which is most stable.

3. Employee Quit by Age Band and Gender

This bar chart displays employee exits segmented by age groups and gender.
It highlights which age ranges are more likely to leave and whether male or female employees have higher attrition in each age band.

4. Employee Quit by Gender

A gender-based pie chart showing attrition comparison between male and female employees.
This helps identify gender-specific trends in workforce exits.

5. Job Satisfaction Gauge

A half-circle gauge visual shows total job satisfaction score.
Lower satisfaction levels can be early indicators of higher attrition risk.

6. Employee Quit by Education Field

This horizontal bar chart indicates how different education fields affect quit rates:

Life Sciences

Medical

Marketing

Technical Degree

Human Resources

Others

This helps HR identify which educational backgrounds have higher resignations.

7. Employee Count by Gender and Marital Status

This clustered bar chart compares employee count for:

Single

Married

Divorced

across male and female groups.
It helps understand how personal and marital factors contribute to employee distribution.

# DAX Formulas Used (Sample)

(These formulas are generic placeholders. Replace with your actual DAX if needed)

Total Employees = COUNT(Employee[EmployeeID])

Employees Quit =
CALCULATE(
    COUNT(Employee[Attrition]),
    KEEPFILTERS(Employee[Attrition] = "Yes")
)

Current Employees =
CALCULATE(
    COUNT(Employee[Attrition]),
    KEEPFILTERS(Employee[Attrition] = "No")
)

Attrition Rate =
DIVIDE([Employees Quit], [Total Employees])

Avg Age = AVERAGE(Employee[Age])

Total Monthly Income = SUM(Employee[MonthlyIncome])

# Conclusion

The Attrition Analysis Dashboard provides clear insights into why employees leave and which groups are most affected. From the analysis, the organization can:

Improve working conditions in departments with high attrition

Focus on engagement programs for specific age groups

Strengthen employee satisfaction to reduce turnover

Use gender and education insights for targeted retention strategies

Adjust HR policies based on marital status trends

By implementing these strategies, the organization can significantly reduce attrition, improve employee morale, and ensure long-term workforce stability.
