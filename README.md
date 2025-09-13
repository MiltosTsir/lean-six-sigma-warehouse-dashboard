# Lean Six Sigma Warehouse Dashboard

This project applies the **Lean Six Sigma DMAIC methodology** to a **simulated warehouse and inventory process**, using **Excel** and **Tableau** for data analysis and visualization.

---

## Project Objective

To reduce **picking errors**, **stockouts**, and **process inefficiencies** in a warehouse environment by analyzing operational data and applying Lean Six Sigma principles.

---

## Project Structure
lean-six-sigma-warehouse-dashboard/
├── data/
│ └── warehouse_inventory_dataset_30000.xlsx # Cleaned dataset (30,000 rows)
├── analysis/
│ ├── excel_kpis_summary.xlsx # KPI calculations & pivot tables
│ └── tableau_dashboard.png # Tableau dashboard screenshot
├── docs/
│ ├── column_descriptions.md # Column-level data dictionary
│ └── dmaic_report.md # Full DMAIC documentation
└── README.md # Project overview


---

## 🛠️ Tools Used

- **Excel** – for KPI calculations, pivot tables, and root cause analysis  
- **Tableau** – for interactive data visualization and dashboard creation

---

## 🔁 Methodology: DMAIC

- **Define** – Identified high picking error rates, stockouts, and fulfillment delays  
- **Measure** – Tracked KPIs: picking error rate, order accuracy, stockouts, lead time  
- **Analyze** – Root causes identified using Pareto charts and segmentation (region, product, shipping method)  
- **Improve** – Suggested layout changes, picker training, reorder point adjustments  
- **Control** – Tableau dashboard implemented to monitor KPIs over time  

See full analysis here: [`docs/dmaic_report.md`](docs/dmaic_report.md)

---

## Dataset & Columns

A **synthetic dataset** with **30,000 simulated warehouse orders**, including:

- Order metadata: `Order ID`, `Order Date`, `Region`, `SKU`
- Inventory metrics: `Inventory Level`, `Reorder Point`, `Stockout`
- Process metrics: `Picking Time`, `Order Accuracy`, `Lead Time`, `Shipping Method`

Full column descriptions: [`docs/column_descriptions.md`](docs/column_descriptions.md)

---

## ✅ Key Outcomes (Simulated)

- 📉 **Picking error rate reduced by 18%**
- 📦 **Stockout incidents decreased by 22%**
- 📈 **Order accuracy improved to 96.5%**
- 📊 **Dashboard built to monitor performance in real time**

---

## ⚠️ Disclaimer

This project uses **synthetic data** generated for **educational and portfolio purposes only**. It does not reflect real customer or business data.
