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

## MEASURE Phase

### Data Source
The dataset used contains **30,000 simulated warehouse orders**, including fields such as:
- Units Ordered vs. Units Shipped
- Inventory Level & Reorder Point
- Picking Time (min)
- Order Accuracy (%)
- Lead Time (days)

Data was generated synthetically to reflect typical warehouse operations and cleaned using Excel. Key fields were validated for consistency and outliers.

---

### Key Performance Indicators (KPIs)

The following metrics were calculated using Excel formulas and pivot tables:

| KPI | Description | Current Value |
|-----|-------------|----------------|
| **Picking Error Rate** | % of orders where shipped units ≠ ordered units | **13.2%** |
| **Order Accuracy (%)** | (Units Shipped / Units Ordered) * 100 | **89.6%** |
| **Stockout Rate** | % of orders where inventory < reorder point | **17.4%** |
| **Avg. Picking Time** | Mean time to pick orders | **15.1 minutes** |
| **Avg. Lead Time** | Days from order to delivery (for completed orders) | **5.3 days** |

---

### Methodology

KPIs were calculated as follows:
- **Order Accuracy (%)** = `(Units Shipped / Units Ordered) * 100`
- **Picking Error** = `1 if Units Ordered ≠ Units Shipped, else 0`
- **Stockout** = `1 if Inventory Level < Reorder Point, else 0`
- **Lead Time** = Difference between Order Date and Ship Date (when applicable)

All calculations were performed in Excel using:
- `IF()`, `COUNTIF()`, `AVERAGE()`, and Pivot Tables
- Filtering by region, category, and shipping method for segmentation

---

### Initial Findings

- High stockout rates in specific SKUs and product categories
- Picking times vary widely between regions
- Higher error rate in **Same Day** orders

These baselines will be used in the Analyze phase to find root causes and improvement opportunities.


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
