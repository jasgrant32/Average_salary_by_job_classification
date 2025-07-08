# Average_salary_by_job_classification

🔍Overview
* This project analyzes average base salaries across job classifications using SQL and Tableau. The goal is to identify trends in salary by grade, role, and employee distribution to inform workforce planning decisions.

💻 Skills Used
* SQL (joins, aggregation, filtering, via phpMyAdmin)
* Relational data modeling
* Data cleaning & preparation
* Data visualization (line, pie and bar charts)
* Github & Tableau public for project organization 

📊 Data Sources
* [Kaggle dataset: Average Salary by Job Classification](https://www.kaggle.com/datasets/sonawanelalitsunil/average-salary-by-job-classification)
* This dataset aggregates information from employment reports, salary surveys, and public job postings.  
* It consists of one main table: `average_salary_by_job_classification`.

🔑 Key Questions Explored
* 💰 Which positions have the highest average base salary?
* 🧑‍💼 Which job classification has the most employees?
* 🏷️ What's the total salary cost by job grade?

🧭 Project Workflow (Start to Finish)
* SQL_syntax_codes.sql – Created database tables and inserted raw CSV data
* Sample_analysis_queries.sql – Wrote SQL queries to explore and analyze key metrics
* charts - Built visualizations using Tableau based on the query results
* summary_findings.txt – Summarized key insights for non-technical audiences

📌 Outcome
* This project demonstrates how SQL, relational databases, and data visualization tools can work together to answer real-world business questions using structured data.
* Basic_queries examples

1) -- Which positions have the highest average base salary?

SELECT position_title, avg_base_salary
FROM job_classifications
ORDER BY avg_base_salary DESC
LIMIT 10;

2) -- Which positions have the hightest average base salary with grade number?

SELECT position_title, avg_base_salary, grade 
FROM job_classifications 
ORDER BY grade, avg_base_salary ASC;

[Salary Trends Across Grades](https://public.tableau.com/app/profile/jasmine.grant/viz/AverageSalarybyJobClassification/SalaryTrendsAcrossGrades)

💡 Recommendation
* Grade levels could be reassessed to ensure they reflect salary fairness
