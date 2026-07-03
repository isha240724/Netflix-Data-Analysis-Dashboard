# Netflix-Data-Analysis-Dashboard
Comprehensive Netflix content data analysis using Power BI and SQL.


## 🚀 Project Overview
This project provides a comprehensive analysis of Netflix's movies and TV shows dataset using SQL and Power BI. The goal was to uncover content trends, growth distribution over the years, and types of media dominating the platform.

## 📊 Key Insights Delivered
* **Content Split:** Movies make up the majority (~69.6%) of Netflix's catalog compared to TV Shows (~30.4%).
* **Growth Trend:** Netflix experienced exponential growth in content additions starting around 2015, peaking between 2018-2020.
* **Interactivity:** Added user-friendly slicers to dynamically filter data by Content Type (Movie/TV Show).

## 💻 Tech Stack Used
* **Power BI Desktop:** For Data Visualization and Dashboard designing.
* **SQL:** For exploratory data analysis (EDA) and data validation.
* **Dataset:** Netflix Movies and TV Shows (CSV format).

## 🔍 SQL Queries Used for Validation
```sql
-- 1. Total Content Count
SELECT COUNT(show_id) AS Total_Titles FROM netflix_table;

-- 2. Movies vs TV Shows Split
SELECT type, COUNT(show_id) AS Count_by_Type 
FROM netflix_table 
GROUP BY type;
