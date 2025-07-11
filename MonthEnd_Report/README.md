# M7 SLA Report – ITSM Monthly Executive Dashboard

## 🧠 Overview

The M7 SLA Report is a monthly business-critical report used by SITA executives to track incident management performance. It shows metrics like the number of SLA met vs missed, response times, resolution times. This is how the different assigned groups performance is measured.

## 🔧 Technologies Used

- SQL Server (T-SQL)
- SSIS (for loading and transformation)
- SQL Server Agent (for job scheduling)
- ITSM Data Tables (e.g., HPD: Help Desk, CTM: People)

## ⚙️ Process Summary

1. Extracted incident data from ITSM landing tables
2. Transformed and cleaned data in the staging layer
3. Loaded into a fact table in the exploitation layer: `FCT_REPORT_SB_ITSM_LAST_INCIDENT10`
4. Built a view to support monthly SLA reporting

## 🚀 Outcome

- Reduced manual reporting effort by 90%
- Ensured on-time delivery of monthly executive reports
- Created a reusable ETL pipeline that can be scheduled via Agent jobs

## 📎 Files attached

- `Sample_SQL_Code.sql`: View script for the report
- `M7_Architecture.png`: ![ETL Architecture](./MReport_architecture.png) 
- `Report_Sample_Screenshot.png`:
