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
Our supply chain has demonstrated resilience and maturity from 2020 to 2024, achieving consistent sales growth and improved operational efficiency. Despite early data anomalies and global disruptions, we have successfully navigated market shifts, optimized inventory and enhanced service levels. Key findings reveal distinct regional preferences and category performance, highlighting clear strategic priorities for future growth and supply chain optimization.


###  Overview of Findings 
- Sales rebounded robustly growing nearly fourfold from 2020 to 2024, demonstrating a mature and resilient supply chain and also overcoming early data anomalies notably in 2021.
  
- The supply chain matured significantly, evidenced by a declining backorder rate from 13% in 2022 to 6.8% in 2024 and stabilized with high order accuracy.

- Clothing and Electronics are the primary growth drivers over 50% of sales with distinct regional preference where Clothing leads in the North/South, Electronics dominates the West and 
  East has balanced demand.

- Order fulfillment shows Accessories have the highest efficiency 71.94%. Clothing leads in volume but with significant pending orders, Electronics experience the highest cancellations 
  and Furniture faces rising pending orders.

- Supplier A dominates overall supply particularly in electronics and accessories, making it crucial for tech-related demand. In contrast, Supplier B maintains the highest inventory 
  with balanced contributions to electronics and clothing, while Suppliers C and Supplier D supllies overall smallest vloume suggesting a niche or specialized role.

- High volumes of pending orders in the West and South  represent a direct risk of conversion to cancellations, locking up significant potential revenue.

- Warehouse capacity is severely underutilized at 34% against a 75% target

- Transportation cost efficiency improved from 14% to about 12% of COGS between 2020 and 2024 despite increased sales volume,
  indicating better route optimization and logistics control.

  


&nbsp;

&nbsp;


# 4. Insights Deep Dive 


###  Sales & Demand Dashboard 


* Early years 2020–2021 reflected pandemic shocks and data irregularities with low sales and high inventory. In 2020 sales remained modest (55k units) despite high inventories (262k 
  units) mainly due to the COVID-19 lockdowns that disrupted logistics and shifted consumer priorities toward essentials. By 2021, sales dropped to an all-time low (761 units), 
  reflecting supply shortages and limited product availability particularly in non-essential categories like clothing and furniture. From 2022 – 2024, we witnessed a strong rebound 
  where sales surged to 192k units with order accuracy exceeding 90% and backorders declining from 13% to 6.8%.  Inventory level were well-optimized, sustaining higher sales without 
  overstocking.

* Clothing and Electronics contributed 27.5% and 6.6% respectively which led the total sales, serving as the company’s main growth drivers. Furniture maintained a steady contribution 
  with a consistent share of 24.9% while Accessories maintain steady but lower sales at around 21%.
  The evolution of our product demand reveals a distinct progression in market leadership. Furniture was the initial sales leader in 2020 but there was a shift to a surge in Electronics 
  during the 2022 tech rebound. Later transitioned into a stable market where apparel (Clothing) emerged as a consistent category leader alongside Electronics from 2023 to 2024.





* Over the five-year period, our sales distribution by region and product category reveals clear market segmentation and evolving consumer preferences.
  The North being the overall leader where demand is well balanced. It is led Clothing and closely followed by Electronics and Furniture with Accessories trailing
  The West stands out as an electronics driven region recording 50,000 unit sold far as surpassing other categories indicating a tech-oriented, urbanized customer based with digital 
  lifestyle needs. 
  In the East, sales are notably even across categories with Electronics (38,803), Furniture (38,739), Accessories (38,580) and Clothing slightly lower with 36,000 unit sold. This 
  balanced demand suggests the region value variety rather than single dominant product type. The South shows a strong preference for Clothing (45,000 units) with other categories 
  trailing which likely driven by fashion-conscious consumers or cultural buying habits.



   

* The efficiency of our supply chain lies a well-coordinated network supplier each playing a distinct role in driving category performance.
  Supplier A is the largest overall unit supplier, primarily focused on Electronics and Accessories, making them vital for tech and accessory categories. Supplier B despite having 
  slightly fewer units than supplier A, has the highest inventory, with strong electronics and clothing focus.
  Supplier C specializes more in Clothing and Electronics but the smallest volume while Supplier D focuses on Clothing and Furniture with lower emphasis on Electronics.

* Our order fulfillment analysis paints a clear picture of category-level operational efficiency and emerging bottlenecks within the supply chain.
  Accessories lead the pack, achieving the highest fulfillment rate (71.94%) and the lowest pending order percentage (18.39%).
  Clothing, while boasting the highest number of fulfilled orders (116,404), also carries a pending order rate of 20.14%.
  Electronics present a different challenge altogether, with the highest cancellation rate (12.63%). These cancellations likely stem from price volatility 
  and heightened competition in the tech market.
  Lastly, Furniture remains a steady contributor but shows operational friction. Despite a moderate cancellation rate (7.86%), its rising pending orders (23.95%) reveal the logistical 
  strain tied to bulky shipments, warehousing delays and transportation lead times.









 
