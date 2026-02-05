📊 SQL Job Market Analysis
📌 Project Overview

This project explores the Data Analyst job market using SQL to analyze salary trends, skill demand, and career optimization strategies. The analysis focuses on remote Data Analyst roles and examines how different technical skills influence salary levels and job market demand.

The goal of this project is to translate workforce data into actionable career insights using relational database analysis.

🎯 Project Objectives

This project answers five key business questions:

What are the highest-paying remote Data Analyst jobs?

What skills are required for top-paying roles?

What skills are most in-demand in the job market?

Which skills are associated with the highest salaries?

Which skills provide the best balance between demand and salary?

🗂 Dataset Description

The project uses a relational dataset consisting of four interconnected tables.

company_dim

Contains company-level metadata.

Column	Description
company_id	Unique company identifier
name	Company name
link	Company website
link_google	Google reference link
thumbnail	Company image or logo
job_postings_fact

Contains job listing details.

Column	Description
job_id	Unique job posting ID
company_id	Company reference
job_title_short	Standardized job title
job_title	Full job title
job_location	Job location
job_work_from_home	Remote work indicator
job_posted_date	Job posting date
salary_year_avg	Average yearly salary
salary_hour_avg	Average hourly salary
skills_dim

Stores skill metadata.

Column	Description
skill_id	Unique skill identifier
skills	Skill name
type	Skill category
skills_job_dim

Bridge table connecting job postings and required skills.

Column	Description
job_id	Job reference
skill_id	Skill reference

🛠 Database Setup
Step 1 — Create Database

Run:

database_setup/1_create_database.sql

Step 2 — Create Tables

Run:

database_setup/2_create_tables.sql


This script creates:

Dimension tables

Fact table

Bridge table

Primary and foreign key relationships

Indexes for query performance

Step 3 — Load Dataset

Run:

database_setup/3_load_data.sql


This loads CSV files into PostgreSQL tables.

📈 Analysis & Findings
💰 Highest Paying Remote Data Analyst Jobs

This query identifies the top-paying remote Data Analyst positions.

Key Findings:

Senior and leadership analytics roles dominate highest salary tiers.

Some remote analyst positions exceed $650,000 annual salary.

High-paying roles exist across multiple industries including healthcare, finance, and technology.

🧠 Skills Required for Top Paying Roles

This analysis maps skills required for high-salary jobs.

Key Findings:

Top-paying roles require cloud computing knowledge.

Big data processing technologies frequently appear.

Programming and automation skills are strongly associated with high salaries.

📊 Most In-Demand Skills

This query identifies skills most frequently requested in Data Analyst job postings.

Top Skills:

SQL

Excel

Python

Tableau

Power BI

Key Insight:

Modern Data Analysts require a hybrid skill set combining data querying, programming, and visualization.

🏆 Highest Paying Skills

This analysis calculates average salary associated with each skill.

Top Salary Skills:

PySpark

Bitbucket

Couchbase

Watson

DataRobot

Key Insight:

Advanced data processing and machine learning automation skills command the highest salaries.

⚖ Optimal Skills (High Demand + High Salary)

This analysis combines salary and demand metrics to identify strategic career skills.

Most Balanced Skills:

SQL

Python

Tableau

Snowflake

Azure

AWS

Key Insight:

Cloud data platforms represent the strongest long-term career investments.

🧠 SQL Techniques Demonstrated

This project demonstrates advanced SQL techniques including:

Common Table Expressions (CTEs)

Multi-table joins

Aggregation and ranking

Filtering and statistical thresholding

Relational data modeling

Workforce analytics

📊 Key Career Insights

SQL remains the most essential skill for Data Analysts.

Cloud computing significantly increases earning potential.

Data Analysts increasingly overlap with data engineering responsibilities.

Visualization tools remain critical for business communication.

⚠ Project Limitations

Salary data varies by region and company size.

Some skills appear multiple times due to dataset categorization.

Analysis focuses only on remote Data Analyst roles.

🚀 Future Improvements

Build interactive dashboards using Power BI or Tableau

Automate data ingestion using Python

Expand analysis across additional job roles

Perform time-series trend analysis
