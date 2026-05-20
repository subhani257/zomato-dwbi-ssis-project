# Zomato Food Delivery Data Warehouse using SQL Server & SSIS



## Overview

This project implements a complete **Data Warehouse and Business Intelligence (DWBI)** solution for analyzing customer behavior in a food delivery platform similar to Zomato.

The solution was developed using:

- SQL Server
- SSIS (SQL Server Integration Services)
- Data Warehouse Design
- ETL Pipelines
- Star Schema Modeling
- Slowly Changing Dimensions (SCD)
- Accumulating Fact Tables

The project processes transactional food delivery session data and transforms it into a dimensional data warehouse for analytical reporting and business insights.

---

# Project Objectives

- Design a complete data warehouse architecture
- Integrate data from multiple heterogeneous data sources
- Develop ETL pipelines using SSIS
- Implement dimensional modeling techniques
- Perform data cleansing and transformation
- Build a star schema for analytical processing
- Implement Slowly Changing Dimensions (SCD)
- Implement an Accumulating Fact Table

---

# Dataset Information

### Dataset Name
Zomato Cart Add-On Sessions Dataset

### Dataset Source
[https://www.kaggle.com/datasets/abdullahsafwan333/zomato-cart-add-on-sessions-dataset](https://www.kaggle.com/datasets/abdullahsafwan333/zomato-cart-add-on-sessions-dataset)

### Dataset Description

The dataset contains 100,000 simulated food delivery sessions modeled after real-world ordering behavior in major Indian cities including:

- Mumbai
- Hyderabad
- Chennai
- Bengaluru

The dataset includes:

- User profiles
- Restaurant information
- Cart details
- Session metadata
- Recommendations
- Transaction data
- Environmental conditions
- Add-on purchasing behavior

---

# Technologies Used

| Technology | Purpose |
|---|---|
| SQL Server | Database Management |
| SSIS | ETL Development |
| SQL | Data Processing |
| Data Warehouse | Analytical Storage |
| Star Schema | Dimensional Modeling |
| Git & GitHub | Version Control |

---

# Architecture

## Data Sources

### Flat Files (CSV)
- Users.csv
- Restaurants.csv

### SQL Server Source Database
- Sessions
- Orders
- Cart
- Recommendations

---

# ETL Architecture Flow

Source Systems → Staging Database → SSIS ETL → Data Warehouse → Analytics

---

# Data Warehouse Design

## Fact Table

### Fact_Order_Session

The fact table stores measurable transaction/session data including:

- Final order value
- Add-on values
- Delivery time
- Engagement score
- Recommendation metrics
- Transaction processing time

---

# Dimension Tables

- Dim_User
- Dim_Restaurant
- Dim_Date
- Dim_Cart
- Dim_Addon
- Dim_Environment

---

# Key Features Implemented

## ETL Development
- Data extraction from multiple sources
- Data cleansing
- Data transformation
- Data loading using SSIS

## Slowly Changing Dimensions (SCD)
Implemented SCD Type 2 for:
- Dim_User
- Dim_Restaurant

## Accumulating Fact Table
Implemented transaction lifecycle tracking using:
- Transaction creation time
- Completion time
- Processing duration

## Data Profiling
Performed data profiling using SSIS Data Profiling Task.

---


# How to Run the Project

1. Restore SQL Server databases
2. Execute SQL scripts
3. Open SSIS project in Visual Studio
4. Configure database connection managers
5. Execute SSIS packages
6. Load data into Data Warehouse

---

# Author

Dulshini W.G.S.

SLIIT - Faculty of Computing

Module:
IT3021 – Data Warehousing & Business Intelligence

---

# License

This project is developed for academic and educational purposes.
