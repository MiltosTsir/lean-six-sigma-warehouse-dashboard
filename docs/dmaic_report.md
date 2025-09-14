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

## MEASURE Phase

In this phase, KPIs were calculated using Excel on a cleaned dataset of 30,000 simulated transactions.

**Key metrics calculated:**

| KPI                  | Value        |
|----------------------|--------------|
| Picking Error Rate   | 8.58%        |
| Stockout Rate        | 25.32%       |
| Order Accuracy       | 91.42%       |
| Avg. Picking Time    | 15 minutes   |
| Avg. Lead Time       | 5.51 days    |

All calculations were performed using Excel formulas and pivot tables.

---

## ANALYZE Phase

Root cause analysis was conducted using Excel tools: pivot tables, Pareto charts, and segmentation by category, region, and shipping method.

### Stockouts by Product Category

| Product Category | Stockout Rate (%) |
|------------------|--------------------|
| Electronics      | 25.85%  
| Toys             | 25.81%  
| Furniture        | 25.17%  
| Apparel          | 24.45%  

**Conclusion**: Electronics and Toys are responsible for the highest stockout rates.

---

### Picking Errors by Product Category

| Product Category | Picking Error Rate (%) |
|------------------|-------------------------|
| Electronics      | 8.68%  
| Toys             | 8.48%  
| Apparel          | 8.44%  
| Furniture        | 3.73%  

**Conclusion**: Errors are concentrated in Electronics, Toys, and Apparel (80/20 rule).

---

### Order Accuracy by Shipping Method

| Shipping Method | Avg. Accuracy (%) | Std. Deviation |
|------------------|-------------------|----------------|
| Same Day         | 99.52%            | 2.52%  
| Standard         | 99.50%            | 2.59%  
| Express          | 99.54%            | 2.44%  

**Conclusion**: Standard shipping shows the highest variability.

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

### Summary of Root Causes

- Stockouts mainly in Electronics and Toys
- Picking errors concentrated in Electronics, Toys, and Apparel
- Process variability in Furniture and Standard shipping
- Low performance in the West region

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

