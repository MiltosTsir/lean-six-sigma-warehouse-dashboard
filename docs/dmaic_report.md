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

| Metric              | Current (Est.) | Target        |
|---------------------|----------------|---------------|
| Picking Error Rate  | ~13%           | < 5%          |
| Stockout Rate       | ~17%           | < 3%          |
| Order Accuracy      | ~89%           | > 95%         |
| Avg. Lead Time      | ~5 days        | < 3 days      |

### Scope
- Inventory management (stock levels, reorder points)
- Order picking process (accuracy, time)
- Shipping preparation (excluding external carrier performance)

### Out of Scope
- Inbound logistics  
- Supplier performance  
- External shipping/delivery delays

---

# 📊 MEASURE Phase

In this phase, KPIs were calculated using Excel on a cleaned dataset of 30,000 simulated warehouse transactions.

## Key Metrics Calculated

| KPI                     | Value        |
|-------------------------|--------------|
| Picking Error Rate (%)  | 8.58%        |
| Stockout Rate (%)       | 25.32%       |
| Order Accuracy (%)      | 91.42%       |
| Avg. Picking Time       | 15 min       |
| Avg. Lead Time          | 5.51 days    |

All calculations were performed using Excel formulas and PivotTables. Financial impact was also estimated based on error costs:

### Financial Impact Overview

| Metric                        | Value (€)     |
|-------------------------------|---------------|
| Total Orders                  | 30,000        |
| Avg. Shipping Cost per Order  | 27.59         |
| Total Shipping Cost           | 827,783.94    |
| Total Picking Errors          | 2,574         |
| Cost per Picking Error        | 5             |
| Cost of Picking Errors        | 12,870        |
| Total Stockouts               | 7,596         |
| Cost per Stockout             | 10            |
| Cost of Stockouts             | 75,960        |

## Additional Insights

- **Shipping Cost per Region/Method** using PivotTables and Conditional Formatting.
- **Order Status Distribution** by shipping method.
- **Picking Time per Product Category**
- **Warehouse Lead Time by Region and Product Category**

All metrics support a full understanding of current process capability and financial impact.

---

# 🔍 ANALYZE Phase

In this phase, root cause analysis was conducted using Excel tools such as:
- PivotTables
- Pareto Charts
- Segmentation by Category, Region, and Shipping Method
- Boxplots and statistical comparisons

## Root Cause Identification

### 🛑 Stockouts by Product Category

| Product Category | Stockout Rate (%) |
|------------------|-------------------|
| Electronics      | 25.85%  
| Toys             | 25.81%  
| Furniture        | 25.17%  
| Apparel          | 24.45%  

**Conclusion**: Electronics and Toys are responsible for the highest stockout rates.

### 📦 Picking Errors by Product Category

| Product Category | Picking Error Rate (%) |
|------------------|------------------------|
| Electronics      | 8.68%  
| Toys             | 8.48%  
| Apparel          | 8.44%  
| Furniture        | 3.73%  

**Conclusion**: Errors are concentrated in Electronics, Toys, and Apparel (Pareto principle 80/20).

#### Pareto Chart – Picking Errors

A Pareto chart was created to visualize the cumulative distribution of picking errors per product category.
<img width="450" height="239" alt="Screenshot 2025-09-14 at 2 36 25 PM" src="https://github.com/user-attachments/assets/9eb69408-8669-4ec1-949d-8714e1998991" />


---

### Order Accuracy by Shipping Method

| Shipping Method | Avg. Accuracy (%) | Std. Deviation |
|------------------|-------------------|----------------|
| Same Day         | 99.52%            | 2.52%  
| Standard         | 99.50%            | 2.59%  
| Express          | 99.54%            | 2.44%  

**Conclusion**: Standard shipping shows slightly higher variability.

---

### Order Accuracy by Product Category

| Product Category | Avg. Accuracy (%) | Std. Deviation |
|------------------|-------------------|----------------|
| Apparel          | 99.53%            | 2.49%  
| Electronics      | 99.52%            | 2.51%  
| Furniture        | 99.51%            | 2.55%  
| Toys             | 99.51%            | 2.52%  

---

### Order Accuracy by Region

| Region | Avg. Accuracy (%) | Std. Deviation |
|--------|-------------------|----------------|
| East   | 99.56%            | 2.43%  
| North  | 99.54%            | 2.46%  
| South  | 99.50%            | 2.53%  
| West   | 99.47%            | 2.63%  

**Conclusion**: The West region shows the lowest performance and highest variability.

---

### 📊 Boxplot Analysis

Boxplots were created to explore variation and potential instability in key performance metrics across different categories and regions.

---

#### 📦 Lead Time per Region

The boxplot for **Lead Time per Region** revealed that the **West region** has the highest variability and several outliers, indicating inconsistent performance and potential delays.

This supports the need for targeted improvements in process standardization or training in that region.

<img width="504" height="242" alt="Screenshot 2025-09-14 at 2 38 42 PM" src="https://github.com/user-attachments/assets/6bceb191-ab62-40e4-aae3-4d1acd7c8627" />

---

#### ⏱ Picking Time per Product Category

The **Picking Time per Product Category** boxplot showed that categories like **Furniture** and **Electronics** had wider interquartile ranges and outliers.

This suggests differences in picking complexity or layout efficiency across categories and justifies further investigation or layout redesign.


<img width="509" height="210" alt="Screenshot 2025-09-14 at 2 39 01 PM" src="https://github.com/user-attachments/assets/6600a1af-60c3-4317-9a2b-fb1118802795" />


---

### 🚚 Shipping Cost vs. Picking Time

Shipping cost was analyzed by **quartiles of picking time**, instead of scatter plots, for better interpretability.

| Picking Time Range | Avg. Shipping Cost (€) |
|---------------------|------------------------|
| 0–10 min            | 27.61  
| 11–15 min           | 27.43  
| 16–20 min           | 27.74  
| 21+ min             | 27.63  

---

## Summary of Root Causes

- **Stockouts** mainly in *Electronics* and *Toys*
- **Picking errors** mostly in *Electronics*, *Toys*, and *Apparel*
- **Variability** observed in *Furniture* category and *Standard* shipping
- **West region** had the lowest order accuracy and highest variability

---

## IMPROVE Phase

Targeted improvements were designed based on the analysis findings:

### 1. Inventory Replenishment Logic
- Adjust reorder points for Electronics and Toys
- Use dynamic demand-based rules for stock levels

### 2. Picking Layout Redesign
- Reorganize zones for high-frequency items
- Implement category-based color zoning

### 3. Barcode Scanning
- Introduce scanning across all shipping methods
- Add a scan-verification step before dispatch

### 4. West Region Training
- Conduct focused training sessions
- Reinforce SOPs and track KPI improvements

### 5. Shipping Method Optimization
- Standardize handling and packing for Standard shipping
- Use visual aids and checklists

### 6. SOP Standardization
- Create consistent processes across region–category combinations
- Document and apply best practices from top-performing regions

---

## CONTROL Phase

To ensure long-term improvement and sustainability, a control plan was established using Excel:

- Created a **KPI monitoring sheet** with visual indicators  
- Included baseline, target, and post-improvement metrics  
- Used conditional formatting to highlight issues in real time  
- Developed weekly report templates to monitor:
  - Picking errors
  - Stockouts
  - Lead times
  - Order accuracy per region

The control tools were fully developed in Excel to enable easy adoption and use without specialized software.

---

## Tools Used

- **Microsoft Excel** – data cleaning, KPI calculations, pivot analysis, control dashboard

---

## Outcome (Simulated)

| Metric                | Before     | After       | Change    |
|-----------------------|------------|-------------|-----------|
| Picking Error Rate    | 10.5%      | 8.58%       | ↓ 18%     |
| Stockout Rate         | 32.5%      | 25.32%      | ↓ 22%     |
| Order Accuracy        | 89%        | 91.42%      | ↑ 2.7%    |
| Avg. Lead Time        | 6.2 days   | 5.51 days   | ↓ 11%     |

---

## Notes

- All data is synthetic and generated for educational purposes only.  
- This project is Excel-only and requires no paid tools or external platforms.

