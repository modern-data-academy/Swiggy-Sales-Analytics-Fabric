# 🍽️ Swiggy Sales Analytics | Microsoft Fabric & Power BI

<p align="center">
  <img src="https://img.shields.io/badge/Microsoft%20Fabric-Analytics-blue?style=for-the-badge&logo=microsoftfabric" alt="Microsoft Fabric"/>
  <img src="https://img.shields.io/badge/Power%20BI-Dashboard-yellow?style=for-the-badge&logo=powerbi" alt="Power BI"/>
  <img src="https://img.shields.io/badge/SQL-T--SQL-orange?style=for-the-badge&logo=microsoftsqlserver" alt="T-SQL"/>
  <img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge" alt="Project Status"/>
</p>

<p align="center">
  <b>🚀 End-to-End Data Engineering | 📊 Business Intelligence | ⚙️ ETL Pipelines</b>
</p>

An end-to-end **Data Engineering and Business Intelligence project** built using Microsoft Fabric, Fabric Lakehouse, Fabric Warehouse, T-SQL, and Power BI to analyze Swiggy restaurant orders, sales, ratings, locations, and customer trends.

This project demonstrates data ingestion, transformation, duplicate management, dimensional modeling, SQL-based data quality checks, and interactive dashboard development.

---

## 📌 Table of Contents

- 🎯 Project Overview
- ✨ Key Features
- 🛠️ Technology Stack
- 🏗️ Project Architecture
- 🗄️ Data Model
- 💻 SQL Development
- 📊 Power BI Dashboard
- 📁 Repository Structure
- 🚀 How to Explore the Project
- 🧠 Skills Demonstrated
- 👩‍💻 Author

---

## 🎯 Project Overview

The objective is to transform raw Swiggy data into structured, analytics-ready datasets and develop an interactive Power BI dashboard to support business analysis and decision-making.

### ✨ Key Features

- 🔄 **Data Engineering:** Built a Lakehouse-to-Warehouse workflow in Microsoft Fabric.
- 🧹 **Data Transformation:** Processed and structured data for analytical reporting.
- 🛡️ **Data Quality:** Used T-SQL to identify duplicates and validate records.
- ⚙️ **Duplicate Management:** Implemented stored procedures and a table-valued function for duplicate detection and removal.
- ⭐ **Dimensional Modeling:** Organized analytical data using fact and dimension tables.
- 📈 **Business Intelligence:** Created interactive Power BI visuals, KPIs, and filters.
- 🌍 **Sales Analytics:** Explored order trends, restaurant ratings, and geographical patterns.

---

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| 🔷 [Microsoft Fabric](https://learn.microsoft.com/fabric/) | Data engineering and analytics platform |
| 🏞️ Fabric Lakehouse | Data storage and processing |
| 🏢 Fabric Warehouse | Structured analytical data storage |
| 💻 [T-SQL](https://learn.microsoft.com/sql/t-sql/) | Data cleaning, validation, and duplicate management |
| 📊 [Power BI](https://powerbi.microsoft.com/) | Interactive dashboards and reporting |
| 🔄 ETL Pipelines | Data movement and workflow orchestration |
| ⭐ Dimensional Modeling | Organizing data for analytical queries |
| 📐 DAX & Power Query | KPI calculations and data transformation, where used in the report |

---

## 🏗️ Project Architecture

```text
📂 Source Data
      |
      ▼
🏞️ Microsoft Fabric Lakehouse
      |
      ▼
🧹 Data Transformation & Cleaning
      |
      ▼
🔄 Lakehouse-to-Warehouse Pipeline
      |
      ▼
🏢 Microsoft Fabric Warehouse
      |
      ├── 📅 dim_date
      ├── 📍 dim_location
      ├── 🍽️ dim_restaurant
      ├── 🥘 dim_dish
      |
      └── 📦 fact_order
               |
               ▼
        📊 Power BI Dashboard
               |
               ▼
        💡 Business Insights
```

---

## 🗄️ Data Model

The project uses a fact-and-dimension structure to support analytical reporting.

### 📐 Dimension Tables

- 📅 `dim_date` — order dates and time-based analysis.
- 📍 `dim_location` — geographical and location-based analysis.
- 🍽️ `dim_restaurant` — restaurant-level analysis.
- 🥘 `dim_dish` — dish and category analysis.

### 📦 Fact Table

- `fact_order` — order-level measures and related dimension keys.

> 📝 Note: Verify table names and relationships against your final Fabric Warehouse schema.

---

## 💻 SQL Development

The T-SQL scripts cover the following activities:

- 🏗️ Creating and querying the `swiggy_project` schema.
- 🔍 Validating record counts across tables.
- 🧹 Identifying duplicate dimension keys and order IDs.
- 📅 Converting source date strings into valid date values.
- 🔢 Removing duplicates using `ROW_NUMBER()` and common table expressions (CTEs).
- ⚙️ Creating stored procedures for duplicate management.
- 🛡️ Creating a table-valued function to report duplicate records across multiple tables.

**Outcome:** Improved data consistency and prepared structured datasets for analytical reporting.

---

## 📊 Power BI Dashboard

The Power BI report provides interactive analysis of Swiggy business performance.

### 📈 Key Analytical Areas

- 💰 Total orders and sales.
- 🍽️ Restaurant and dish performance.
- ⭐ Ratings and rating counts.
- 📍 Location-based comparisons.
- 📅 Date-based sales and order trends.
- 🎛️ Interactive slicers, filters, and KPI cards.

### 🖼️ Dashboard Preview

Add your dashboard screenshot to the `screenshots` folder and display it here:

```markdown
![Swiggy Sales Analytics Dashboard](screenshots/dashboard-overview.png)
```

---

## 📁 Repository Structure

```text
swiggy-sales-analytics-fabric/
│
├── 📄 README.md
│
├── 💻 sql/
│   └── T-SQL-Swiggy.sql
│
├── 🏢 warehouse/
│   └── Swiggy_DW/
│
├── 🔄 pipelines/
│   └── LH-to-WH/
│
├── 📊 powerbi/
│   └── Swiggy-Analysis.pbix
│
└── 🖼️ screenshots/
    └── dashboard-overview.png
```

*Organize the uploaded files into these folders. The actual extracted Warehouse and pipeline file structure may differ from this example.*

---

## 🚀 How to Explore the Project

1. 📥 Download or clone this repository.
2. 💻 Review the SQL scripts to understand data cleaning and duplicate-management logic.
3. 🏢 Explore the Warehouse project files, including tables, functions, and stored procedures.
4. 🔄 Review the Lakehouse-to-Warehouse pipeline definitions.
5. 📊 Open `Swiggy-Analysis.pbix` in Power BI Desktop.
6. 🔌 Configure your own Fabric connections and workspace settings if you want to reproduce the workflow.

### 📋 Prerequisites

- Microsoft Fabric workspace with appropriate permissions.
- Power BI Desktop.
- Compatible SQL environment for reviewing or executing scripts.
- Access to the relevant source data and connections to reproduce the pipeline.

---

## 🧠 Skills Demonstrated

<p>
  <img src="https://img.shields.io/badge/Data%20Engineering-0078D4?style=flat-square" alt="Data Engineering"/>
  <img src="https://img.shields.io/badge/Microsoft%20Fabric-512BD4?style=flat-square&logo=microsoftfabric" alt="Microsoft Fabric"/>
  <img src="https://img.shields.io/badge/Power%20BI-F2C811?style=flat-square&logo=powerbi&logoColor=black" alt="Power BI"/>
  <img src="https://img.shields.io/badge/SQL-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white" alt="SQL"/>
  <img src="https://img.shields.io/badge/ETL%20Pipelines-008272?style=flat-square" alt="ETL Pipelines"/>
  <img src="https://img.shields.io/badge/Data%20Modeling-6A5ACD?style=flat-square" alt="Data Modeling"/>
  <img src="https://img.shields.io/badge/Data%20Quality-228B22?style=flat-square" alt="Data Quality"/>
  <img src="https://img.shields.io/badge/Business%20Intelligence-FF8C00?style=flat-square" alt="Business Intelligence"/>
</p>

- 🔄 ETL and Data Pipeline Development
- 🏞️ Microsoft Fabric Lakehouse and Warehouse
- 💻 SQL and T-SQL
- 🧹 Data Cleaning and Data Quality
- 📐 Dimensional Modeling
- ⚙️ Duplicate Detection and Removal
- 📊 Power BI Dashboard Development
- 💡 Business Intelligence and Data Analytics

---

## 👩‍💻 Author

### Riya Thokal

🚀 Aspiring Data Engineer | Microsoft Fabric | SQL | Power BI | Python

- 🐙 **GitHub:** [riyathokalofficial-stack](https://github.com/riyathokalofficial-stack)
- 💼 **LinkedIn:** [riya-engineer](https://www.linkedin.com/in/riya-engineer/)

---

⭐ **If you find this project useful, consider giving the repository a star!**

💬 Feedback and suggestions are always welcome.
