# Column Descriptions: Warehouse Inventory Dataset

This file explains each column in the `warehouse_inventory_dataset_30000.xlsx` file and how it contributes to the Lean Six Sigma analysis of the warehouse process and inventory.

| Column Name | Description | What It Shows / How to Use It |
|-------------|-------------|-------------------------------|
| **Order ID** | Unique identifier for each customer order. | Used to track individual transactions; useful for order-level analysis. |
| **Order Date** | Date when the order was placed. | Useful for trend analysis over time, seasonality, and demand forecasting. |
| **Region** | Geographic region where the order was shipped. (North, South, East, West) | Helps identify regional performance and possible logistics bottlenecks. |
| **Product Category** | Product classification (e.g., Electronics, Furniture, Food). | Useful for ABC analysis and category-specific KPIs. |
| **SKU** | Unique product identifier (Stock Keeping Unit). | Enables SKU-level inventory and picking analysis. |
| **Units Ordered** | Quantity of units requested in the order. | Input for calculating demand, inventory planning, and order fulfillment metrics. |
| **Units Shipped** | Quantity of units actually shipped to the customer. | Used to calculate picking accuracy and fulfillment performance. |
| **Order Status** | Final status of the order (Completed, Delayed, Cancelled). | Important for identifying service level and delays. Can be used in Pareto or control chart. |
| **Shipping Method** | Mode of delivery (Standard, Express, Same Day). | Allows analysis of cost and lead time per shipping type. |
| **Shipping Cost (€)** | Cost of shipping the order in euros. | Can be analyzed in relation to region, method, weight, and speed of fulfillment. |
| **Warehouse Picking Time (min)** | Time (in minutes) spent on picking this order in the warehouse. | Core process metric — used to analyze efficiency, identify bottlenecks, and calculate takt time. |
| **Inventory Level** | Stock quantity available at the time of order processing. | Used to assess inventory sufficiency and stockout risk. Enables analysis of inventory turnover. |
| **Reorder Point** | Minimum stock level at which a new order should be placed. | Used to trigger replenishment; critical for avoiding stockouts. |
| **Stockout** | Binary (0/1): 1 if inventory level is below reorder point, 0 otherwise. | Indicator for supply problems. Used in waste analysis and to improve safety stock strategies. |
| **Picking Error** | Binary (0/1): 1 if shipped units ≠ ordered units, 0 if exact match. | Key quality metric for warehouse operations. Useful in Pareto analysis and Six Sigma defect tracking. |
| **Order Accuracy (%)** | Percentage of correct fulfillment: (Units Shipped / Units Ordered) * 100. | Shows fulfillment accuracy. Important Lean metric for quality and customer satisfaction. |
| **Lead Time (days)** | Number of days from order to delivery (only for Completed orders). | Measures service speed. Can be used in process capability (Cp, Cpk), and to identify delays. |
