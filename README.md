# ⛏️ Mining Operations Dashboard – Fleet Management Analytics

## Executive Summary
This project demonstrates the design and development of an end-to-end Business Intelligence solution for mining fleet operations.
Using a synthetic PostgreSQL database, the project integrates **SQL**, **Power BI**, **Power Query**, and **DAX** to analyze productivity, operational efficiency, route performance, operator effectiveness, and fleet reliability through interactive dashboards designed for decision-making.

# Using the database
1. Create a database named mine.
2. Run mine.sql.
3. Open mining.pbix.
4. Update the data source if necessary.

# Dashboard Overview
This dashboard was designed to answer key operational questions related to:
- Fleet productivity
- Material movement
- Route efficiency
- Operator performance
- Cycle time analysis
- Fleet reliability
- Operational KPIs
The solution follows a star-schema data model and provides interactive dashboards for operational and executive decision-making.

# Business Questions
The dashboard answers questions such as:
- Which trucks are the most productive?
- Which routes maximize productivity while minimizing fuel consumption?
- How do weather conditions affect operational performance?
- Which operators consistently achieve the highest productivity?
- Where is most of the cycle time consumed?
- Which trucks experience the highest delay and breakdown rates?

# Dashboard Pages

## 1. Executive Overview
High-level operational KPIs including:
- Total Production
- TPH
- Fuel per Ton
- Average Cycle Time
- Delay Rate
- Breakdown Rate
- Daily Production Trend

## 2. Fleet Productivity & Reliability
Fleet-level performance analysis including:
- Top 5 Trucks by TPH
- Bottom 5 Trucks by TPH
- Top 5 Trucks by Breakdown Rate
- Top 5 Trucks by Delay Rate

## 3. Operational Performance Analysis
Production analysis by:
- Material
- Weather
- Shift
Including:
- Production
- TPH
- Fuel Consumption

## 4. Route Efficiency Analysis
Route comparison including:
- Production by Route
- Route Distance
- TPH
- Fuel per Ton
Business interpretation highlighting the most efficient haul route.

## 5. Operator Productivity & Performance
Operator comparison including:
- Top 5 Operators
- Bottom 5 Operators
Performance matrix displaying:
- TPH
- Average Cycle Time
- Delay Rate
for each haul route.

## 6. Cycle Time Analysis
Detailed cycle decomposition including:
- Average Cycle Time by Route
- Cycle Components
- Average Cycle Time by Weather
- Average Cycle Time by Shift

## 7. Fleet Maintenance & Reliability
Fleet reliability analysis including:
- Top 10 Trucks by Breakdown Events
- Top 10 Trucks by Idle Time
- Breakdown Rate vs Effective TPH
- Delay Rate vs Effective TPH

## 8. Project Summary
Project documentation including:
- Business Objective
- KPIs
- Business Questions
- Key Findings

# Data Model
The project follows a **Star Schema**.
Fact Table
- Fact Cycle
Dimension Tables
- Truck
- Operator
- Material
- Route
- Location
- Weather
- Shift

# Technologies
- PostgreSQL
- SQL
- Power BI
- Power Query
- DAX

# Key Performance Indicators (KPIs)
- Total Production
- Tons per Hour (TPH)
- Fuel per Ton
- Average Cycle Time
- Delay Rate
- Breakdown Rate
- Production by Material
- Production by Route

# Key Findings
- FC01 → CH01 is the most productive haul route while maintaining the lowest fuel consumption.
- Rain negatively impacts fleet productivity and increases average cycle time.
- Loaded travel represents the largest portion of the haul cycle.
- Operator performance remains highly consistent across the fleet.
- Breakdown rates show relatively low variability between trucks.
- Fuel efficiency is strongly associated with haul distance and material type.

# Repository Structure

```
Mining/
│
├── db/
│   └── mine.sql
│
├── powerbi/
│   └── mining.pbix
│
├── Images/
│   ├── Executive Overview.png
│   ├── Fleet Productivity.png
│   ├── Operational Analytics.png
│   ├── Route Efficiency.png
│   ├── Operator Performance.png
│   ├── Cycle Time Analysis.png
│   └── Fleet Maintenance.png
│
└── README.md
```
# Skills Demonstrated
- SQL Data Analysis
- Data Modeling
- Star Schema Design
- Power BI Dashboard Development
- DAX Measures
- KPI Design
- Business Intelligence
- Data Visualization
- Operational Analytics

# Author
**Guillermo Jofre**

Data Analyst | Business Intelligence | SQL | Power BI | Python

[LinkedIn](https://www.linkedin.com/in/guillermo-jofre/)

[GitHub](https://github.com/Jofregf)

[Portfolio](https://portfolio-jofregf.vercel.app/)