# Real-Time Bike-Sharing Analytics & Regional Performance
This project transforms raw, flat-file operational data from a multi-city bike-sharing system into a structured Star Schema data model in Power BI. The analysis provides actionable insights into bike availability, station health, and regional infrastructure needs to optimize urban mobility.

Project Objectives:
Data Modeling: Convert single flat-file datasets into a central Fact table and related Dimension tables (Station, Date) to improve reporting efficiency.
Operational Monitoring: Categorize stations based on real-time stock levels (e.g., Critical Empty, Low Stock, Healthy) to identify service gaps.
Geospatial Analysis: Visualize station distribution and regional density using Latitude and Longitude coordinates.
Trend Tracking: Implement Year-to-Date (YTD) and Monthly analysis to understand seasonal shifts and hourly peaks in bike usage.

Key Insights & Recommendations:
Redistribution Priority: Identified urgent needs in Marseille and Lyon, where high counts of "Critical Empty" stations (129 and 419 respectively) hinder service reliability.
Infrastructure Expansion: Prescribed physical capacity increases for Lyon and Valence due to consistent "Critical Full" saturations at high-traffic hubs.
Data Quality: Established a quality audit protocol to filter out "Test" and "Warehouse" locations, ensuring operational dashboards reflect only public-facing stations.
Peak Demand: Analysis of hourly trends shows a significant availability peak around 15:00, with high utilization drops observed during morning and evening rush hours.

Technical Stack:
Power BI: Data modeling, DAX measures (YTD, Occupancy %), and interactive visualization.
Power Query: ETL processes including unpivoting, data type standardization, and removal of non-operational test records.

Data Schema:
The model utilizes a Star Schema featuring:
Fact_Bikes: Centralizes availability metrics, bike counts, and timestamps.
Dim_Station: Contains geographic and descriptive attributes for 1,028 active stations.

Dim_Date: A dedicated calendar table to support time-intelligence calculations.
