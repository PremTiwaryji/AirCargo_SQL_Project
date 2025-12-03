# AirCargo_SQL_Project
MySQL project - Air Cargo Analysis (schema, queries, ER diagram, 4 CSV datasets)
# Air Cargo Analysis — MySQL Project

**Project Type:** SQL / Data Analysis  
**Author:** Prem Tiwary  
**Date:** December 4, 2025

---

## Project Overview
This project analyzes airline passenger, route, and ticket datasets to derive operational and business insights. The work includes database design (ER diagram), schema creation, data import, optimized SQL queries, views, stored procedures, and performance tuning.

**Files included**
- `MySQL_Aircargo_Project.pdf` — Full project report (ER diagram, queries, explanations).  
- `customer.csv` — Customer master data.  
- `passengers_on_flights.csv` — Flight passenger records.  
- `routes.csv` — Route and flight information.  
- `ticket_details.csv` — Ticketing data (price, class, date).

---

## Key Skills Demonstrated
- Relational database design & ER modeling  
- Data cleaning & bulk import (`LOAD DATA INFILE`)  
- Advanced SQL: `JOIN`, `GROUP BY`, `HAVING`, window functions, `ROLLUP`  
- Stored procedures, functions, and views implementation  
- Query optimization: indexes and `EXPLAIN` plan analysis  
- Business insights extraction and actionable recommendations

---

## Business Insights (Summary)
- High-demand routes and passenger distribution by route/class.  
- Revenue analysis by travel class and by customer (identified high-value customers).  
- Route classification: Short / Intermediate / Long distance; identified long-haul profitable routes (> 2000 miles).  
- Customer segmentation: Business-class and brand-preference (e.g., Emirates) lists.

---

## How to run / reproduce
1. Create a MySQL database (MySQL 8.x recommended).  
2. Create tables using the DDL in the PDF or run the provided `CREATE TABLE` statements.  
3. Import CSV files using `LOAD DATA INFILE` or your preferred database client import.  
4. Create the indexes and stored procedures as described in the PDF.  
5. Run queries and stored procedures for analysis.

---

## Notable Queries / Scripts
- `sp_get_passengers_between_routes(start, end)` — Return passengers for a route range (with table existence check).  
- `sp_routes_over_2000()` — List routes with distance > 2000 miles.  
- `v_business_customers` — View of business-class customers.  
- Indexing scripts to speed up route lookups (e.g., `CREATE INDEX idx_passengers_routeid ON passengers_on_flights(route_id);`)

---

## Contact
**Name:** Prem Tiwary  
**Email:** premtiwary7050@gmail.com 
**LinkedIn:** www.linkedin.com/in/prem-tiwary

---

## License
This repository is for demonstration and learning purposes. Feel free to reuse the code with attribution.

