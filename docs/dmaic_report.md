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

## Analyze Phase

During this phase, we analyzed the root causes behind warehouse inefficiencies using Excel pivot tables, Pareto charts, and descriptive statistics. The main focus areas were:

- Stockouts
- Picking Errors
- Order Accuracy Variability

---

### Pareto Analysis – Stockouts by Product Category

A Pareto-style analysis was performed on stockouts across product categories.

| Product Category | Stockout Rate (%) |
|------------------|--------------------|
| Electronics      | 25.85%  
| Toys             | 25.81%  
| Furniture        | 25.17%  
| Apparel          | 24.45%  

> **Electronics** and **Toys** show the highest stockout rates, indicating potential issues with demand forecasting or reorder point logic.

---

### Pareto Analysis – Picking Errors by Product Category

| Product Category | Picking Error Rate (%) |
|------------------|-------------------------|
| Electronics      | 8.68%  
| Toys             | 8.48%  
| Apparel          | 8.44%  
| Furniture        | 3.73%  

> The majority of picking errors come from **Electronics**, **Toys**, and **Apparel**, suggesting a classic 80/20 Pareto pattern.  
> **Furniture** performs significantly better, which may indicate simpler picking processes or better-trained staff.

---

### Order Accuracy Variability by Shipping Method

| Shipping Method | Avg. Accuracy (%) | Std. Deviation |
|------------------|-------------------|----------------|
| Same Day         | 99.52%            | 2.52%  
| Standard         | 99.50%            | 2.59%  
| Express          | 99.54%            | 2.44%  

> **Standard shipping** shows the highest variability, suggesting that this method may lack process consistency or experience higher error pressure due to volume.

---

### Order Accuracy Variability by Product Category

| Product Category | Avg. Accuracy (%) | Std. Deviation |
|------------------|-------------------|----------------|
| Apparel          | 99.53%            | 2.49%  
| Electronics      | 99.52%            | 2.51%  
| Furniture        | 99.51%            | 2.55%  
| Toys             | 99.51%            | 2.52%  

> **Furniture** products have the highest variance, possibly due to product size, handling complexity, or packaging inconsistencies.

---

### Order Accuracy Variability by Region

| Region | Avg. Accuracy (%) | Std. Deviation |
|--------|-------------------|----------------|
| East   | 99.56%            | 2.43%  
| North  | 99.54%            | 2.46%  
| South  | 99.50%            | 2.53%  
| West   | 99.47%            | 2.63% 

> The **West region** consistently underperforms in both accuracy and stability.  
This region should be prioritized for improvement in process training, layout optimization, or staffing evaluation.

---

### Summary of Root Causes Identified

- High stockouts in **Electronics** and **Toys**
- High picking error rates in **Electronics**, **Toys**, and **Apparel**
- Increased variability in **Furniture category** and **Standard shipping method**
- **West region** has both the lowest order accuracy and the highest variance

> These findings will guide the next phase (Improve), where targeted solutions will be designed for maximum impact.

---

## IMPROVE Phase

### Objective

Based on the findings from the Analyze phase, several targeted actions were proposed to reduce errors, stockouts, and process variability in the warehouse operation.

---

### 1. Inventory Replenishment Logic (Stockouts)

**Pivot Table**: Stockouts by Product Category  
- **Observation**: Electronics (25.65%) and Toys (25.49%) had the highest share of stockouts.  
- **Action**: Adjust the **Reorder Point logic** for these categories based on actual consumption patterns.

Suggested Improvement:
- Implement demand-based dynamic reorder points using moving average or safety stock buffers.
- Review SKU-level inventory policies for high-rotation items.

---

### 2. Picking Errors & Layout Redesign

**Pivot Table**: Picking Errors by Product Category  
- **Observation**: Electronics (25.41%) and Furniture (25.14%) contribute the most to overall picking errors.  
- **Action**: Redesign layout to optimize frequently picked items and reduce human error.

Suggested Improvement:
- Place high-frequency items closer to packing stations.
- Color-code shelving zones by category for faster access.

---

### 3. Barcode Scanning Justification

**Pivot Table**: Picking Errors by Shipping Method  
- **Observation**: All shipping methods (Express, Same Day, Standard) have nearly equal error distribution (~33%).  
- **Action**: Introduce barcode scanning across all methods to ensure item verification before shipment.

Suggested Improvement:
- Pilot barcode scanning in one zone and scale based on impact on accuracy and time.
- Integrate scan confirmation step in the workflow to avoid manual picking errors.

---

### 4. Targeted Training for West Region

**Pivot Table**: Order Accuracy by Region  
- **Observation**: The **West region** had the **lowest average accuracy (99.47%)** and the **highest StdDev (2.65%)**.  
- **Action**: Launch focused training sessions in the West warehouse.

Suggested Improvement:
- Reinforce SOPs through weekly workshops and on-the-floor coaching.
- Track improvements over time using KPIs and dashboard alerts.

---

### 5. Shipping Method Optimization

**Pivot Table**: Order Accuracy by Shipping Method  
- **Observation**: **Standard shipping** had the highest standard deviation (2.59%) in order accuracy.  
- **Action**: Standardize packing and handling for standard shipments to reduce inconsistency.

Suggested Improvement:
- Create visual checklists for standard method packers.
- Add final inspection step before dispatch for bulk standard orders.

---

### 6. Standardization & SOPs

**Pivot Table**: Order Accuracy by Product Category × Region  
- **Observation**: Variability across category–region combinations (e.g., Toys–West).  
- **Action**: Develop **Standard Operating Procedures (SOPs)** for all key combinations.

Suggested Improvement:
- Use best-performing region as benchmark and replicate across others.
- Document processes using flowcharts and integrate into onboarding/training.

---

### Summary of Proposed Improvements

| Improvement Area           | Action Item                                      |
|---------------------------|--------------------------------------------------|
| Inventory Management      | Dynamic reorder points, demand-based planning    |
| Picking Layout            | Zone redesign, fast-moving item prioritization   |
| Error Prevention          | Barcode scanning system implementation           |
| Regional Training         | West region accuracy training                    |
| SOP Standardization       | Standard processes across product-region combos  |
| Shipping Optimization     | Streamlined handling for Standard method         |

---

> 📈 These actions will be monitored in the **Control Phase** through KPIs and real-time dashboards built in Tableau.



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
