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

## 🔍 Analyze Phase

During this phase, we analyzed the root causes behind warehouse inefficiencies using Excel pivot tables, Pareto charts, and descriptive statistics. The main focus areas were:

- Stockouts
- Picking Errors
- Order Accuracy Variability

---

### 📊 Pareto Analysis – Stockouts by Product Category

A Pareto-style analysis was performed on stockouts across product categories.

| Product Category | Stockout Rate (%) |
|------------------|--------------------|
| Electronics      | 25.85%  
| Toys             | 25.81%  
| Furniture        | 25.17%  
| Apparel          | 24.45%  

> **Electronics** and **Toys** show the highest stockout rates, indicating potential issues with demand forecasting or reorder point logic.

---

### 📦 Pareto Analysis – Picking Errors by Product Category

| Product Category | Picking Error Rate (%) |
|------------------|-------------------------|
| Electronics      | 8.68%  
| Toys             | 8.48%  
| Apparel          | 8.44%  
| Furniture        | 3.73%  

> The majority of picking errors come from **Electronics**, **Toys**, and **Apparel**, suggesting a classic 80/20 Pareto pattern.  
> **Furniture** performs significantly better, which may indicate simpler picking processes or better-trained staff.

---

### 📐 Order Accuracy Variability by Shipping Method

| Shipping Method | Avg. Accuracy (%) | Std. Deviation |
|------------------|-------------------|----------------|
| Same Day         | 99.52%            | 2.52%  
| Standard         | 99.50%            | 2.59%  
| Express          | 99.54%            | 2.44%  

> **Standard shipping** shows the highest variability, suggesting that this method may lack process consistency or experience higher error pressure due to volume.

---

### 🏷️ Order Accuracy Variability by Product Category

| Product Category | Avg. Accuracy (%) | Std. Deviation |
|------------------|-------------------|----------------|
| Apparel          | 99.53%            | 2.49%  
| Electronics      | 99.52%            | 2.51%  
| Furniture        | 99.51%            | 2.55%  
| Toys             | 99.51%            | 2.52%  

> **Furniture** products have the highest variance, possibly due to product size, handling complexity, or packaging inconsistencies.

---

### 🌍 Order Accuracy Variability by Region

| Region | Avg. Accuracy (%) | Std. Deviation |
|--------|-------------------|----------------|
| East   | 99.56%            | 2.43%  
| North  | 99.54%            | 2.46%  
| South  | 99.50%            | 2.53%  
| West   | 99.47%            | 2.63% ✅  

> The **West region** consistently underperforms in both accuracy and stability.  
This region should be prioritized for improvement in process training, layout optimization, or staffing evaluation.

---

### ✅ Summary of Root Causes Identified

- High stockouts in **Electronics** and **Toys**
- High picking error rates in **Electronics**, **Toys**, and **Apparel**
- Increased variability in **Furniture category** and **Standard shipping method**
- **West region** has both the lowest order accuracy and the highest variance

> These findings will guide the next phase (Improve), where targeted solutions will be designed for maximum impact.

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
