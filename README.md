# Ferns-N-Petals-fnp-Sales-Fulfillment-Analysis-Dashboard

An interactive, end-to-end Excel analytics dashboard designed to monitor revenue performance, order volume, customer spending patterns, and delivery lead times across product categories, occasions.

# Project Overview

This project analyzes sales and operational data for Ferns N Petals (fnp) to uncover key business insights regarding peak revenue periods, top-selling product categories, regional order distribution, and fulfillment efficiency.

By leveraging Power Query for data ETL (Extract, Transform, Load) and Power Pivot (DAX) for relational data modeling and KPI calculation, this dashboard translates raw transactional data into actionable executive insights.

## Dataset used-

- <a href="https://github.com/riya1234000/Ferns-N-Petals-fnp-Sales-Fulfillment-Analysis-Dashboard/blob/main/customers.csv">Dataset</a>
- <a href="https://github.com/riya1234000/Ferns-N-Petals-fnp-Sales-Fulfillment-Analysis-Dashboard/blob/main/orders.csv">Dataset</a>
- <a href="https://github.com/riya1234000/Ferns-N-Petals-fnp-Sales-Fulfillment-Analysis-Dashboard/blob/main/products.csv">Dataset</a>

- CUSTOMERS:-  Customer_ID,	Name,	City,	Contact_Number,	Email,	Gender.

- ORDERS: Order_ID,	Customer_ID,	Product_ID,	Quantity,	Order_Date,	Order_Time,	Delivery_Date,	Delivery_Time,	Location,	Occasion,	Month Name,	Hour (ORDER TIME),	DIFF_ORDER_DELIEVERY,	Hour (DELIEVERY TIME),	Price (INR),	ORDER_DAY,	REVENUE.

- PRODUCTS: Product_ID,	Product_Name,	Category,	Price (INR),	Occasion.

## Tools Used: 

Microsoft Excel (Data Cleaning, Power Query, Power Pivot, Data Modelling, Pivot Tables, Data Visualization, Slicers, KPI Cards).


## Dashboard interactive 

<img src="[https://github.com/riya1234000/Ferns-N-Petals-fnp-Sales-Fulfillment-Analysis-Dashboard/blob/main/Screenshot%202026-09-30%20014242.png]" alt="Image Description" width="1000">

#  Data Cleaning & Transformation Data Cleaning:

Standardized date and time formats across transactional records.Cleared duplicates, missing values, and validated key integrity across tables.Feature Engineering & Calculated Columns:Month Extraction: Derived Order Month from order dates to track monthly sales performance and peak seasons.   Hour Extraction: Extracted Order Hour and Delivery Hour to pinpoint peak transaction and dispatch windows.   Fulfillment Latency: Computed the total turnaround time (Delivery Time - Order Time) to measure fulfillment speed.   Price Fetching: Integrated the Price column from the PRODUCTS table into the orders context using data modeling relationships/lookups to enable revenue calculations.  

#  Data Modeling

To build a scalable and structured analytics foundation, a robust relational data model (Star Schema / Relational Model) was created connecting all three datasets:Relationships Established: Linked the central fact table (ORDERS) to dimension tables (CUSTOMERS and PRODUCTS) using CustomerID and ProductID keys.Calculated Measures & Aggregates: Built measures for Total Revenue, Average Order Value, Total Orders, and Average Delivery Time.   Filter Context & Referential Integrity: Configured one-to-many relationships to ensure seamless cross-filtering across dimensions when using slicers and timelines

#  Dashboard Features & Visualizations KPI Summary Cards:

High-level visual metrics display Total Revenue (₹ 35,20,984.00), Total Orders (1,000), Average Delivery Time (5.53 Days), and Average Customer Spend (₹ 3,520.98).   Interactive Slicers & Timelines: Dynamic filters for Occasions, Categories, Order Dates, and Delivery Timelines.   Trend & Geographic Analysis: Charts analyzing Revenue by Occasion, Category, Month, Top 5 Products, Top 10 Cities, and Revenue by Hour. 

## Key Performance Metrics (KPIs)
- Total Revenue Generated: ₹ ₹ 35,20,98  across analyzed order batches.

- Total Orders Analyzed: ₹ 1000 orders processed across key regions.

- Average Order Value (AOV): ₹3520.984 per customer transaction.

- Average Delivery Lead Time: 5.53 days from order placement to customer delivery.

## Key Business Insights
1. Festival Seasonality Drives Peak Revenue  festive Anniversary emerged as the top revenue-generating occasion, contributing ₹6,74,634 (19.16% of total revenue).

Valentine's Day (₹3,31,930) with (9.43%) and Diwali (₹3,13,783) with (8.91%) followed as steady year-round revenue drivers.

Monthly Peak: August delivered the highest revenue share (₹7,37,389) with (20.94%). 
## Sweets & Festive Hampers Lead Product Categories
Colors generated the highest category revenue at (₹10,05,645) followed by Soft Toys (₹7,40,831) and Sweets (₹7,33,842).

Category mix highlights strong demand for edible Colors over standard perishable items like Soft Toys during peak months.

## Strategic Growth 
Supply Chain Optimization for August: Lock in stock and logistics agreements by mid-July to handle the 20.94% annual sales concentration in August.

AOV Growth via Bundling: Create pre-packaged anniversary bundles combining Colors & Sweets to leverage the ₹3,520.98 benchmark AOV.

Fulfillment Speed Reduction: Optimize the current 5.53-day average lead time by establishing local fulfillment hubs in top revenue-generating cities.

