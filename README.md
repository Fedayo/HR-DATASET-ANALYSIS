# 📊 HR Attrition Analysis Project

## 🔍 Overview
This project analyzes employee attrition data to understand the factors that contribute to employee turnover. Using a dataset from an HR department, I created a comprehensive Power BI dashboard to visualize key metrics such as attrition rate, total number of employee and so on

## 🎯 Objectives
The main goals of this project are:
- To identify trends and patterns in employee attrition.
- To provide actionable insights for HR managers to reduce turnover.
- To gain hands-on experience with Power BI for data visualization.

## 🗂️ Dataset Information
The dataset (`HR_Attrition_Dataset.csv` contains the following columns:
- `EmployeeID`: Unique identifier for each employee.
- `Attrition`: Indicates whether an employee left (Yes/No).
- `Department`: Department where the employee worked (e.g., Sales, HR, IT).
- `Education`: Education level of the employee (e.g., Bachelor's, Master's).
- `AgeBracket`: Age range of the employee (e.g., 20-30, 30-40).
- `Gender`: Gender of the employee (Male/Female).
- `YearsAtCompany`: Number of years the employee has worked at the company.
- `JobSatisfaction`: Employee satisfaction rating (1-5) and so much more

## 💻 Data Cleaning and Preparation
I performed the following data cleaning steps:
1. Removed duplicates and null values.
2. Standardized age brackets and education levels.
3. Created calculated columns for metrics like `Current Employee Count` and `Attrition Rate` using DAX in Power BI.

### **SQL Script for Data Preparation**
Here's a snippet of the SQL script used for initial data cleaning:

```sql
-- Removing duplicates and handling missing values
SELECT DISTINCT *
FROM hr_data
WHERE attrition IS NOT NULL;
