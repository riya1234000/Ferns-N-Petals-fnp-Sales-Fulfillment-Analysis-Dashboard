# Ferns-N-Petals-fnp-Sales-Fulfillment-Analysis-Dashboard

An interactive, end-to-end Excel analytics dashboard designed to monitor revenue performance, order volume, customer spending patterns, and delivery lead times across product categories, occasions, and geographic regions.

# Project Overview

This project analyzes sales and operational data for Ferns N Petals (fnp) to uncover key business insights regarding peak revenue periods, top-selling product categories, regional order distribution, and fulfillment efficiency.

By leveraging Power Query for data ETL (Extract, Transform, Load) and Power Pivot (DAX) for relational data modeling and KPI calculation, this dashboard translates raw transactional data into actionable executive insights.

#  Project Datasets
CUSTOMERS:Customer demographics, location details, and unique IDs.

ORDERS: Order transactions, timestamps (order time, delivery time), and core order metrics.

PRODUCTS: Catalog items, categories, and unit price reference data. 

#  Data Cleaning & Transformation Data Cleaning:

Standardized date and time formats across transactional records.Cleared duplicates, missing values, and validated key integrity across tables.Feature Engineering & Calculated Columns:Month Extraction: Derived Order Month from order dates to track monthly sales performance and peak seasons.   Hour Extraction: Extracted Order Hour and Delivery Hour to pinpoint peak transaction and dispatch windows.   Fulfillment Latency: Computed the total turnaround time (Delivery Time - Order Time) to measure fulfillment speed.   Price Fetching: Integrated the Price column from the PRODUCTS table into the orders context using data modeling relationships/lookups to enable revenue calculations.  

#  Data Modeling

To build a scalable and structured analytics foundation, a robust relational data model (Star Schema / Relational Model) was created connecting all three datasets:Relationships Established: Linked the central fact table (ORDERS) to dimension tables (CUSTOMERS and PRODUCTS) using CustomerID and ProductID keys.Calculated Measures & Aggregates: Built measures for Total Revenue, Average Order Value, Total Orders, and Average Delivery Time.   Filter Context & Referential Integrity: Configured one-to-many relationships to ensure seamless cross-filtering across dimensions when using slicers and timelines

#  Dashboard Features & Visualizations KPI Summary Cards:

High-level visual metrics display Total Revenue (₹ 35,20,984.00), Total Orders (1,000), Average Delivery Time (5.53 Days), and Average Customer Spend (₹ 3,520.98).   Interactive Slicers & Timelines: Dynamic filters for Occasions, Categories, Order Dates, and Delivery Timelines.   Trend & Geographic Analysis: Charts analyzing Revenue by Occasion, Category, Month, Top 5 Products, Top 10 Cities, and Revenue by Hour. 

#  Key Insights & Findings
Peak Hours: High order volumes occur during specific hours, allowing for targeted logistics staffing.

Fulfillment Bottlenecks: Identified the average delivery delay between placement and doorstep arrival.

Product Performance: Top-performing product lines were highlighted based on integrated price and volume data.
