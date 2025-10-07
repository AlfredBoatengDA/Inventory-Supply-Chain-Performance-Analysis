# Inventory-Supply-Chain-Performance-Analysis
![](https://github.com/AlfredBoatengDA/Inventory-Supply-Chain-Performance-Analysis/blob/main/Inventory%20analysis%20image.webp)




## Table of Content

- [Project Overview](Project-Overview)
- [Data Structure Overview](Data-Structure-Overview)
- [Executive Summary](Executive-Summary)
- [Insights Deep Dive](Insights-Deep-Dive)
- [Recommendation](Recommendations)
- [Conclusion](Conclusion)


&nbsp;


# Project Overview
The Supply Chain Inventory Performance Analysis project aims to evaluate the operational and cost efficiency of a multi-regional distribution network involving four primary suppliers and multiple warehouses servicing the North, South, East and West regions. This analysis focuses on assessing order fulfillment efficiency, uncovering regional and category based demand patterns, measuring warehouse utilization and analyzing key cost components including transportation expenses and cost of goods sold (COGS). The ultimate goal is to provide actionable insights that optimize inventory management, enhance supply chain responsiveness and improve overall cost effectiveness.

### Problem Statement
1) Investigates how crop yields have evolved over time across
2) Identifying Yield Performance Across Regions
3) Assessing the Impact of Pesticide Use on Crop Productivity
4) How climate factors like rainfall levels and temperature impact crop suitability and yield


&nbsp;



# Data Structure Overview
| Column Name | Description |
| **Column Name**               | **Description**                                                                     |
| ----------------------------- | ----------------------------------------------------------------------------------- |
| **Date**                      | The date when the order transaction occurred.                                       |
| **Region**                    | The geographical region of operation (e.g., North, South, East, West).              |
| **Category**                  | The type of product category (e.g., Electronics, Clothing, Furniture, Accessories). |
| **Supplier**                  | The vendor responsible for fulfilling the order (Supplier A, B, C, or D).           |
| **Warehouse**                 | The warehouse location where the inventory is stored and processed.                 |
| **Order Status**              | The current status of the order (Fulfilled, Pending, or Cancelled).                 |
| **Units Sold**                | The total number of product units sold per transaction or record.                   |
| **Inventory Level**           | The available stock quantity at the time of reporting.                              |
| **Transportation Cost**       | The cost incurred for transporting goods from suppliers to warehouses or customers. |
| **Order Accuracy**            | A Boolean indicator showing whether the order was correctly fulfilled (TRUE/FALSE). |
| **Lead Time (Days)**          | The average number of days taken from order placement to fulfillment.               |
| **Backorder**                 | A Boolean value indicating whether the product was on backorder (TRUE/FALSE).       |
| **Cost of Goods Sold (COGS)** | The total production or procurement cost of goods sold within the given period.     |
| **Average Inventory**         | The mean value of inventory held during a specific period.                          |
| **Warehouse Capacity**        | The total storage capacity available in the warehouse.                              |

&nbsp;


#### Data Source
* The dataset used in this project is titled "Yield_df" and is provided in CSV format. 
* Data was sourced from Kaggle



#### Tools
 - Python - Data Cleaning & Exploratory Data Analysis can be downloaded [here](https://github.com/AlfredBoatengDA/Agriculture-Projects/blob/main/Data%20Cleaning.ipynb)
 - SQL Server - Perform analysis,  utilized to inspect, perform quality checks
                and also target various business questions [here](https://github.com/AlfredBoatengDA/Agriculture-Projects/blob/main/SQL%20Analysis%20and%20Queries.sql)
 - Power BI - Creating reports & interacting with visuals can be downloaded  [here](https://github.com/AlfredBoatengDA/Agriculture-Projects/blob/main/Crop%20Yield%20Analysis%20Power%20BI%20Dashboard.pbix)


# Executive Summary

 
