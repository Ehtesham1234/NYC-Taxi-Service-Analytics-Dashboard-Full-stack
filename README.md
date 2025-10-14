# 🚖 NYC Taxi Trip Analytics Dashboard

A comprehensive Power BI analytics project providing end-to-end insights into New York City taxi operations, designed for city analysts, business strategists, and data science learners to explore trip patterns, revenue trends, and customer behavior across boroughs and service zones.

---

## 🧭 Short Description / Purpose

The NYC Taxi Trip Analytics Dashboard visualizes millions of real trip records from New York City to uncover how ride volume, fare dynamics, tipping behavior, and service zones interact over time.  
It enables analysts to monitor performance, identify demand trends, and understand rider habits across boroughs.

---

## ⚙️ Tech Stack

The project combines data engineering, statistical cleaning, and interactive business intelligence using the following stack:

| Tool / Technology | Purpose |
|--------------------|----------|
| 🐍 **Python (Pandas)** | Data cleaning, preprocessing, and exploratory analysis |
| 💻 **Jupyter Notebook** | Interactive environment for cleaning, visualization, and testing logic |
| 🗄️ **PostgreSQL** | Structured data storage, SQL cleaning, joins, and data modeling |
| 📊 **Power BI Desktop** | Interactive data visualization and dashboard creation |
| 🧠 **DAX (Data Analysis Expressions)** | Calculated measures, KPIs, and conditional logic |
| 🧹 **Power Query** | Data transformation and load layer |
| 📁 **CSV Dataset Files** | Input format for trip, location, and weather data |

---

## 🗂️ Data Source

**Source:**  
New York City Taxi & Limousine Commission (TLC) Trip Record Data (January–March 2023)

**Dataset Details:**
- ~9 million trip records from Yellow Taxi service.  
- Key columns: pickup/drop-off timestamps, fare amount, tip, total amount, distance, passenger count, borough, and service zone.  
- Supplemented with NYC OpenWeather API for rainy-day tagging and analysis.

**Storage & Modeling:**  
Data was first cleaned in Python (Jupyter) using Pandas, then loaded into PostgreSQL for advanced transformations and relationships between:
- `trip_data` (main table)
- `zone_lookup` (borough mapping)
- `weather_data` (rainy day flag)

---

## 💡 Features / Highlights

### 🧩 Business Problem
City transportation departments and analysts lack a consolidated, visual tool to evaluate taxi operations and customer patterns across NYC.  
Raw data is difficult to interpret, leading to missed insights in demand forecasting, tipping behavior, and borough-level revenue performance.

### 🎯 Goal of the Dashboard
To deliver a data-driven visualization tool that:
- Tracks trip volume, revenue, and tip performance across months and boroughs.  
- Evaluates weather impact on customer tipping.  
- Monitors operational KPIs like fare/mile and trip duration.  
- Empowers stakeholders to make data-informed policy and operational decisions.

---

## 📈 Walkthrough of Key Visuals

| Section | Visual Type | Description |
|----------|--------------|--------------|
| **Top KPI Row** | KPI Cards | Displays total trips (9M), total revenue ($242M), avg fare/mile (5.37), avg duration (15.04 min), avg tip %, and total airport fees (316K). |
| **Revenue by Month & Day** | Column Chart | Shows daily revenue trend, revealing dips and peaks across January–March. |
| **Trips by Quarter** | Area Chart | Highlights recovery in trip counts post-February slowdown. |
| **Tip Comparison on Rainy Days** | Line Chart | Demonstrates correlation between rain and higher average tipping behavior. |
| **Revenue by Service Zone** | Pie Chart | Identifies dominant zones (Manhattan and Airport areas). |
| **Revenue by Borough** | Map Visual | Geographical view of borough-wise performance. |
| **Dynamic Slicers (Left Panel)** | Dropdown Filters | Allow filtering by month, borough, and location for interactive exploration. |

---

## 💼 Business Impact & Insights

- **Operational Efficiency:** Helps identify under-performing zones or months for strategic focus.  
- **Behavioral Insight:** Shows that rainy weather positively impacts tipping by ~3%.  
- **Revenue Distribution:** Manhattan and airport zones generate nearly half of total revenue.  
- **Decision Enablement:** Supports taxi regulators and city analysts in optimizing fare structures and route strategies.

---

## 🖼️ Screenshots / Demos
**Dashboard Overview**  
*(Insert image link once uploaded to repo — e.g. `![Dashboard Screenshot](assets/NYC_Taxi_Dashboard.png)`)*

---

## 📂 Files Included

- `data_cleaning.ipynb` → Python notebook for preprocessing  
- `database_schema.sql` → PostgreSQL schema and transformations  
- `NYC_Taxi_Analytics.pbix` → Final Power BI report file  
- `assets/` → Exported visuals for documentation  

---

## 🏁 Project Summary

**Impact:**  
Delivered a scalable, interactive Power BI dashboard that visualizes over **9 million trips**, connecting **data engineering + analytics + visualization** in one workflow.  

It serves as a **case study for real-world data cleaning, SQL modeling, and business storytelling** through Power BI.

---
