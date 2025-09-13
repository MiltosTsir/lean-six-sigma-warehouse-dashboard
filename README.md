# Lean Six Sigma Warehouse Dashboard

This project applies the **Lean Six Sigma DMAIC methodology** to a simulated warehouse and inventory process, using **Excel** and **Tableau** for data analysis and visualization.

---

## Project Objective

To reduce picking errors, stockouts, and process inefficiencies in a warehouse environment by analyzing operational data and applying Lean Six Sigma principles.

---

## Project Structure
lean-six-sigma-warehouse-dashboard/
│
├── data/
│ └── warehouse_inventory_dataset_30000.xlsx
│
├── analysis/
│ ├── excel_kpis_summary.xlsx # Excel with KPIs and pivot tables
│ └── tableau_dashboard.png # Tableau dashboard screenshot
│
├── docs/
│ ├── column_descriptions.md # Column-level data dictionary
│ └── dmaic_report.md # Lean Six Sigma DMAIC project summary
│
└── README.md


---

## Tools Used

- **Excel** – for KPI calculations, pivot tables, and root cause analysis
- **Tableau** – for data visualization and dashboard creation

---

## Methodology: DMAIC

- **Define:** Problem – high error rates and stockouts
- **Measure:** KPIs like picking error, stockout rate, order accuracy, lead time
- **Analyze:** Root causes via Pareto and trend analysis
- **Improve:** Layout changes, warehouse training, reorder point logic
- **Control:** Tableau dashboard monitors KPIs over time

See full analysis here: [`docs/dmaic_report.md`](docs/dmaic_report.md)

---

## Dataset & Columns

Synthetic dataset with 30,000 orders including:
- Order date, region, SKU, inventory levels
- Shipping method, cost, errors, stockouts

Column descriptions: [`docs/column_descriptions.md`](docs/column_descriptions.md)

---

## Key Outcomes (Simulated)

- ✅ Picking error rate reduced by 18%
- ✅ Stockout incidents decreased by 22%
- ✅ Order accuracy improved to 96.5%
- ✅ Dashboard built to monitor improvements in real time

---

## Disclaimer

This project uses **synthetic data** generated for educational and portfolio purposes only.


