# Supply - Chain - Project-

Supply Chain Analytics

An end-to-end supply chain analytics project focused on inventory management, product performance, warehouse operations, supplier performance, demand analysis, and forecast accuracy.

The project takes raw supply chain data through a complete analytics workflow using SQL Server, Python, Jupyter Notebook, and Power BI. The goal is to convert operational data into meaningful business insights that can support inventory planning, procurement, supplier management, and supply chain decision-making.

«Note: The GitHub repository contains the key project files and documentation. If you want to explore the complete project, including the dataset, SQL scripts, Python notebook, Power BI dashboard, and supporting files, download the ZIP file provided in the repository.»

---

Project Overview

Supply chain teams need to continuously monitor inventory, product demand, warehouse operations, supplier performance, and forecast accuracy. Poor visibility into these areas can lead to stockouts, excess inventory, inefficient warehouse operations, and inaccurate purchasing decisions.

This project analyzes supply chain data to understand:

- Product and inventory performance
- Demand and sales patterns
- Inventory turnover
- Warehouse performance
- Supplier lead times and performance
- Forecast accuracy and demand deviations
- Inventory buffer requirements
- Buffer-to-demand relationships
- Potential replenishment requirements
- Opportunities for supply chain optimization

The project follows an end-to-end analytics workflow:

Kaggle Dataset → Data Preparation → SQL Server → SQL Analysis → Python EDA → Power BI → Business Insights

---

Business Objectives

The main objectives of the project are to:

- Analyze overall supply chain performance
- Identify high- and low-performing products
- Evaluate inventory levels and inventory turnover
- Monitor warehouse performance
- Analyze supplier lead times and delivery performance
- Compare actual demand with forecasted demand
- Measure forecast accuracy using MAE and MAPE
- Analyze inventory buffer requirements
- Identify products that may require replenishment
- Understand demand and inventory trends
- Support data-driven supply chain decisions

---

Tools and Technologies

Tool| Purpose
SQL Server| Database creation, table creation, data loading, and analysis
SQL| Analytical queries, business calculations, and reusable views
Python| Exploratory data analysis and data investigation
Pandas| Data manipulation and analysis
Jupyter Notebook| EDA and data visualization
Power BI| Interactive reporting and dashboard development
DAX| Measures and calculated metrics
Power Query| Data preparation and transformation
GitHub| Project documentation and version control

---

Power BI Dashboard

The Power BI dashboard provides an interactive view of supply chain performance across different analytical areas.

1. Home

The Home page serves as the main navigation page for the dashboard.

It provides access to:

- Executive Overview
- Inventory & Product
- Warehouse Performance
- Supplier Performance
- Forecast Performance

Each section can be accessed through the corresponding navigation buttons.

---

2. Executive Overview

The Executive Overview provides a high-level view of supply chain performance.

Key metrics and analyses include:

- Total Units Sold
- Average Inventory
- Average Supplier Lead Time
- Forecast MAPE
- Stockout Rate
- Monthly Demand
- Inventory Turnover
- Promotion Impact

This page is designed to provide a quick understanding of the overall supply chain position before moving into detailed analysis.

---

3. Inventory & Product

This section focuses on product-level performance and inventory management.

The analysis includes:

- Units Sold by SKU
- Inventory Performance
- Inventory Turnover
- Average Inventory
- Inventory Buffer
- Buffer-to-Demand Ratio
- Reorder Status
- Replenishment Analysis
- Product-level demand patterns

The purpose is to identify products that require closer inventory monitoring and understand how inventory levels relate to demand.

---

4. Warehouse Performance

This section analyzes warehouse-level operational performance.

The analysis covers:

- Warehouse performance
- Warehouse utilization
- Inventory availability
- Operational efficiency
- Warehouse-level comparisons

This helps identify differences in warehouse operations and inventory handling.

---

5. Supplier Performance

The Supplier Performance section evaluates supplier-related metrics.

The analysis focuses on:

- Supplier lead time
- Supplier performance
- Delivery-related performance
- Supplier comparisons
- Operational reliability

The objective is to understand supplier-level differences and identify areas that may require closer monitoring.

---

6. Forecast Performance

This section focuses on demand forecasting and forecast deviations.

Key areas include:

- Actual Demand
- Forecasted Demand
- Forecast MAE
- Forecast MAPE
- Forecast deviations
- Inventory Buffer
- Buffer-to-Demand Ratio

This analysis helps evaluate how closely forecasted demand matches actual demand and how forecast deviations may affect inventory planning.

---

Key Metrics

Mean Absolute Error (MAE)

MAE measures the average absolute difference between actual demand and forecasted demand.

A lower MAE generally indicates that the forecast is closer to actual demand.

Mean Absolute Percentage Error (MAPE)

MAPE measures forecast error relative to actual demand and expresses it as a percentage.

A lower MAPE generally indicates better forecast accuracy, although MAPE can be problematic when actual demand values are zero or very small.

Inventory Turnover

Inventory turnover measures how efficiently inventory is being utilized relative to demand or sales over a given period.

Higher turnover can indicate faster inventory movement, while very low turnover may indicate slow-moving inventory. The appropriate level depends on the business and product category.

Inventory Buffer

Inventory buffer represents additional inventory maintained to help manage uncertainty in demand and supply.

It can help reduce the risk of stockouts when actual demand or supplier lead times differ from expectations.

Buffer-to-Demand Ratio

The buffer-to-demand ratio compares inventory buffer with demand.

This provides additional context for understanding whether the available buffer is relatively large or small compared with expected demand.

Stockout Rate

Stockout rate measures the proportion of demand or inventory situations where the required stock was unavailable.

A higher stockout rate can indicate potential issues with inventory planning, replenishment, forecasting, or supplier availability.

---

SQL Analysis

The SQL component provides the structured data foundation for the project.

The SQL workflow includes:

1. Creating the SQL Server database
2. Creating the required tables
3. Loading the supply chain dataset
4. Performing analytical queries
5. Creating reusable SQL views
6. Preparing data for reporting and further analysis

The SQL folder contains:

SQL/
├── 01_CreateDatabase.sql
├── 02_CreateTables.sql
├── 03_LoadData.sql
├── 04_AnalysisQueries.sql
└── 05_Views.sql

The analytical queries are used to investigate inventory, products, warehouses, suppliers, demand, and forecasting-related metrics.

---

Python and Exploratory Data Analysis

The project includes a Jupyter Notebook for exploratory data analysis.

The EDA process covers:

- Dataset structure and data types
- Missing-value analysis
- Descriptive statistics
- Distribution analysis
- Product analysis
- Inventory analysis
- Supplier analysis
- Warehouse analysis
- Demand and sales analysis
- Forecast-related analysis
- Data visualization
- Identification of important patterns and relationships

The main notebook is:

01_EDA.ipynb

Python and Pandas were used to explore the dataset and investigate patterns before building the final Power BI reporting layer.

---

Dataset

The dataset used in this project was obtained from Kaggle.

Dataset: High-Dimensional Supply Chain Inventory Dataset
Author: ziya07
Source: Kaggle

The dataset is used for analytical and educational purposes.

The original dataset is available on "Kaggle" (https://www.kaggle.com/datasets/ziya07/high-dimensional-supply-chain-inventory-dataset?utm_source=chatgpt.com).

---

Project Structure

Supply Chain Analytics/
│
├── Data/
│   └── Source supply chain dataset
│
├── SQL/
│   ├── 01_CreateDatabase.sql
│   ├── 02_CreateTables.sql
│   ├── 03_LoadData.sql
│   ├── 04_AnalysisQueries.sql
│   └── 05_Views.sql
│
├── screenshots/
│   ├── Home
│   ├── Executive Overview
│   ├── Inventory & Product
│   ├── Warehouse Performance
│   ├── Supplier Performance
│   └── Forecast Performance
│
├── 01_EDA.ipynb
├── Supply Chain Dashboard.pbix
└── README.md

For the complete project structure and all supporting files, download the ZIP file from the repository.

---

Project Workflow

The project follows this workflow:

Kaggle Dataset
       ↓
Data Preparation
       ↓
SQL Server Database
       ↓
SQL Analysis & Views
       ↓
Python Exploratory Data Analysis
       ↓
Power BI Data Model
       ↓
Power BI Dashboard
       ↓
Business Insights

Each stage serves a specific purpose, from structuring the raw data to producing an interactive reporting and analysis layer.

---

Key Business Insights

The project provides a framework for analyzing:

- Products with different demand and inventory patterns
- High- and low-inventory-turnover products
- Products requiring closer inventory monitoring
- Warehouse-level performance differences
- Supplier lead-time variations
- Forecast deviations
- Inventory buffer levels relative to demand
- Potential replenishment requirements
- Areas for inventory optimization

These insights can support decisions related to inventory planning, procurement, supplier management, warehouse operations, and demand forecasting.

---

How to Use the Project

SQL Analysis

Open the SQL scripts in SQL Server Management Studio and execute them in the following order:

01_CreateDatabase.sql
02_CreateTables.sql
03_LoadData.sql
04_AnalysisQueries.sql
05_Views.sql

Make sure the required dataset files are available before running the data-loading script.

Python EDA

Open:

01_EDA.ipynb

using Jupyter Notebook or JupyterLab.

Run the notebook cells sequentially to reproduce the exploratory analysis.

Power BI Dashboard

Open:

Supply Chain Dashboard.pbix

using Power BI Desktop.

Depending on the local setup, you may need to update the data source or file paths before refreshing the report.

---

Project Deliverables

The project includes:

- Interactive Power BI dashboard
- Python exploratory data analysis
- SQL Server database scripts
- SQL analytical queries
- SQL views
- Source dataset
- Power BI dashboard screenshots
- Project documentation

For the complete set of project files, download the ZIP file available in the repository.

---

Author

Prakhar Varshney
Data Analyst | SQL | Python | Power BI

---

Project Purpose

This project demonstrates an end-to-end approach to supply chain analytics, combining database management, SQL analysis, Python-based exploration, and Power BI reporting to turn operational data into structured business insights.
