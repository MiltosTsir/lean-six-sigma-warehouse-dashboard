# DMAIC Report: Lean Six Sigma Warehouse & Inventory Optimization

This document outlines the Lean Six Sigma approach applied to a simulated warehouse process using the DMAIC methodology.

---

## Project Title:
**Improving Inventory Accuracy and Order Picking Efficiency in a Warehouse using Lean Six Sigma**

---

## DEFINE Phase

### Process Description
The process under analysis is the **warehouse order fulfillment** workflow, focusing on the stages of **order picking and inventory availability**. Each order is picked, packed, and shipped from warehouse stock based on customer demand.

### Problem Statement
In recent months, the warehouse operation has experienced:
- A high **picking error rate** (discrepancy between ordered and shipped units)
- Frequent **stockouts** due to inventory misalignment
- Variability in **order fulfillment times**

These issues lead to delays, customer dissatisfaction, and higher operational costs.

### Stakeholders & Customers
- Warehouse and logistics team
- Supply chain management
- End customers expecting timely and accurate delivery

### Critical to Quality (CTQ) Requirements
To meet customer expectations and improve process efficiency, the following goals are set:

| **Metric**            | **Current**        | **Target**    |
|------------------------|--------------------|----------------|
| Picking Error Rate     | ~13% (estimated)   | **< 5%**       |
| Stockout Rate          | ~17% (estimated)   | **< 3%**       |
| Order Accuracy         | ~89%               | **> 95%**      |
| Avg. Lead Time         | ~5 days            | **< 3 days**   |

### Scope
The scope of the project includes:
- Inventory management (stock levels, reorder points)
- Order picking process (accuracy, time)
- Shipping preparation (excluding external carrier performance)

### Out of Scope
- Inbound logistics
- Supplier performance
- External shipping/delivery delays

---

## MEASURE Phase

### Data Source

The dataset includes **30,000 synthetic warehouse transactions**, designed to simulate real-world logistics operations. Key fields include:

- **Units Ordered** vs. **Units Shipped**
- **Inventory Level** & **Reorder Point**
- **Warehouse Picking Time (min)**
- **Order Accuracy (%)**
- **Lead Time (days)**

Data was cleaned and analyzed in **Excel**, using formulas, filters, and pivot tables. Outliers and unrealistic values (e.g., order accuracy > 100%) were identified and excluded to ensure data quality.

---

### Key Performance Indicators (KPIs)

The following KPIs were defined to measure current warehouse performance:

| **KPI**                | **Description**                                              | **Value**        |
|------------------------|--------------------------------------------------------------|------------------|
| **Picking Error Rate** | % of orders with incorrect picking (errors in quantity/item) | **8.58%**        |
| **Order Accuracy**     | % of orders delivered with exactly correct quantity          | **91.42%**       |
| **Stockout Rate**      | % of orders affected by inventory shortages (stockouts)      | **25.32%**       |
| **Avg. Picking Time**  | Average time to complete picking per order                   | **15.00 minutes**|
| **Avg. Lead Time**     | Average time from order placement to delivery                | **5.51 days**    |

> *All calculations were performed using Excel formulas. Cleaned values were used for final KPI reporting.*

---

### Methodology

The KPIs were calculated using logic-based Excel formulas and pivot tables. Key formula logic includes:

- **Order Accuracy (%)** = `(Units Shipped / Units Ordered) * 100`
- **Picking Error** = `1` if `Units Ordered ≠ Units Shipped`, else `0`
- **Stockout** = `1` if `Inventory Level < Reorder Point`, else `0`
- **Lead Time** = `Order Date – Ship Date` (for completed orders only)

All calculations were performed using:
- Excel functions: `IF()`, `COUNTIF()`, `AVERAGE()`, and Pivot Tables
- Filtering and segmentation by: `Region`, `Product Category`, `Shipping Method`

---

### Initial Findings

Baseline analysis revealed the following insights:

- Stockouts are highly concentrated in specific SKUs and product categories  
- Picking times show high variability across regions  
- Higher error rates observed in Same-Day shipping orders  

These insights will guide the Analyze Phase, where root causes will be identified and prioritized for improvement.


---

## Suggested Improvements (Improve)

Based on the analysis, we proposed:

- Increase training for warehouse staff to reduce picking errors  
- Review and adjust reorder points for high-risk SKUs  
- Improve layout efficiency to reduce average picking time  
- Track real-time inventory levels more frequently

---

## Control Plan (Control)

To ensure sustained improvement:

- Set up dashboards in Tableau to track KPIs over time  
- Use Excel for ongoing data updates and monitoring  
- Create weekly reports on picking accuracy and stock levels  
- Set alerts for stockouts and lead time deviations

---

## Tools Used

- **Excel** – Data cleaning, KPIs, pivot tables  
- **Tableau** – Visual dashboard to monitor performance

---

## Outcome (Simulated)

- Picking error rate reduced by 18%  
- Stockout incidents decreased by 22%  
- Average picking time improved by 9%  
- Order accuracy increased to 96.5%

---

*Note: All data is simulated and used for educational purposes only.*
