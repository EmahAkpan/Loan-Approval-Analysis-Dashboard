# Loan-Approval-Analysis-Dashboard
This analysis explores key factors influencing loan approvals using a dataset that includes demographic, financial, and application-specific information.  
 Loan Prediction Analysis – README

📝 Project Overview
This project focuses on analyzing a loan prediction dataset to uncover patterns and insights that affect loan approvals. It explores demographic factors, financial indicators, and risk factors to support data-driven decisions in financial services, especially loan underwriting. The final goal is to help stakeholders understand which factors most influence loan approval outcomes.

🎯 Objective
To analyze loan approval patterns using demographic and financial features such as gender, age, income, credit score, and loan purpose. The project aims to identify key factors influencing loan approval and provide actionable insights using Excel features like formulas, PivotTables, charts, and slicers.

📝 Dataset Description
The dataset includes the following columns:
Column Name	Description
Gender	Male / Female
Age	Applicant's age
Age Group	Derived category: Middle age / Older
Credit Score	Numeric value indicating credit rating
Annual Income	Applicant’s yearly income
Loan Purpose	Type of loan requested
Loan Status	Approved / Not Approved

🛠️ Tools and Features Used in Excel
Power Query: Data cleaning and transformation

IF functions: Age grouping, binary classification

PivotTables & PivotCharts: Summary analysis

Slicers: For interactive filtering

Scatter Plots: Visualize correlation

Bar & Column Charts: Comparison by category

🔢 Key Excel Formulas (Code)
1. Creating Age Group Column
excel
Copy
Edit
=IF([@Age] < 45, "Middle Age", "Older")
2. Binary Conversion for Loan Status
excel
Copy
Edit
=IF([@LoanStatus]="Approved", 1, 0)
3. Count of Approved vs Not Approved
Using COUNTIFS:

excel
Copy
Edit
=COUNTIFS(Gender, "Male", LoanStatus, "Approved")
=COUNTIFS(Gender, "Female", LoanStatus, "Not Approved")
4. Percentage Approval Rate by Purpose
excel
Copy
Edit
=COUNTIFS(LoanPurpose, "Home", LoanStatus, "Approved") / COUNTIF(LoanPurpose, "Home")
Format cell as Percentage.

📊 Visualizations Created
Pivot Chart: Gender vs Loan Approval

Bar Chart: Loan Purpose Approval Rate

Stacked Column Chart: Gender & Age vs Loan Status

Scatter Plot: Annual Income vs Credit Score

Slicers: Applied to filter Education status and Employment level

📈 Sample Pivot Table Structure
Row: Gender
Column: Loan Status
Values: Count of Loan Status
Filter: Age Group or Purpose
Use % of Column Total to get approval percentages.

📌 Summary of Insights
Approval by Gender:

Male: 69.35%

Female: 70.72%

Age Group Impact:

Middle-aged applicants are slightly higher loan approval rate than Older and young ones.

Loan Purpose Approval:

Highest: Home (71.39%)

Lowest: Car (67.91%)

Credit Score & Income:

Scatter plot shows a trend: Higher credit scores and income lead to more approvals.

✅ Recommendations
Prioritize applicants with higher credit scores and income.

Consider reviewing policies for car loan approvals due to lower success rates.

Encourage loan types like Home and Personal which have higher approval rates.

📂 Suggested Folder Organization


LoanPredictionExcelProject/
│
├── Data/
│   └── cleaned_loan_data.xlsx
│
├── Analysis/
│   └── pivot_summary.xlsx
│
├── Visuals/
│   ├── gender_vs_approval_chart.png
│   ├── loan_purpose_bar_chart.png
│   ├── scatter_income_credit.png
│
├── Report/
│   └── loan_analysis_summary.docx
│
└── README.xlsx (this file)

**Conclusion**
The analysis provides valuable insights into the loan approval process. Employment status, credit score, gender and annual income emerged as strong predictors of approval,high education marginally improved approval chances while,. Loan purposes showed a minor influence on approval butl Loans for home and personal purposes had the highest approval rates. These findings can help financial institutions optimize their lending strategies, mitigate risk, and improve inclusivity in the approval process.

<img width="4718" height="77" alt="image" src="https://github.com/user-attachments/assets/853ee7c4-b1ad-498f-89d0-dc44fcb92f9c" />

