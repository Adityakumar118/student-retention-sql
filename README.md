# 🎓 Student Retention Analysis with SQL

## 🧩 Objective
To identify student dropout patterns and suggest retention strategies.

## 🔧 Tools Used
- MySQL for querying
- Excel for summary reporting

## 📊 Key Insights
- Dropouts were highest in the 2nd year (35%).
- Students with GPA below 6.0 had a 48% higher dropout rate.

## 📁 Files
- `retention_queries.sql` – All SQL queries used
- `student_data.csv` – Raw data (mocked for privacy)

## 🔍 Sample Query
```sql
SELECT Year, COUNT(*) AS Dropouts
FROM student_data
WHERE status = 'Dropped'
GROUP BY Year;
