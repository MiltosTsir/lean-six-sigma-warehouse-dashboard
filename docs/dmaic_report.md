# DMAIC Report: Lean Six Sigma Warehouse & Inventory Optimization

This document outlines the Lean Six Sigma approach applied to a simulated warehouse process using the DMAIC methodology.

---

## Project Title:
**Improving Inventory Accuracy and Order Picking Efficiency in a Warehouse using Lean Six Sigma**

---

## Problem Statement (Define)

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

| Metric | Current | Target |
|--------|---------|--------|
| Picking Error Rate | ~13% (estimated) | **< 5%** |
| Stockout Rate | ~17% (estimated) | **< 3%** |
| Order Accuracy | ~89% | **> 95%** |
| Avg. Lead Time | ~5 days | **< 3 days** |

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

## Metrics & Data (Measure)

We used a dataset of 30,000 warehouse order records with the following key metrics:

- **Picking Error Rate** = % of orders with discrepancies between ordered and shipped units  
- **Stockout Rate** = % of orders where inventory level < reorder point  
- **Order Accuracy (%)**  
- **Lead Time (days)** for completed orders  
- **Warehouse Picking Time (minutes)**

---

## Root Cause Analysis (Analyze)

Using tools like Pareto charts and basic data segmentation, we identified:

- High error rates in specific product categories and regions  
- Delays concentrated in same-day shipping methods  
- Stockouts driven by low reorder point thresholds or high demand spikes

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
