# Lean Six Sigma Warehouse Dashboard

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Last Commit](https://img.shields.io/github/last-commit/MiltosTsir/lean-six-sigma-warehouse-dashboard)](https://github.com/MiltosTsir/lean-six-sigma-warehouse-dashboard/commits/main)

## Project Overview

This project applies the **Lean Six Sigma DMAIC methodology** to a **simulated warehouse and inventory management process**, using **Microsoft Excel** for data analysis, KPI tracking, and root cause exploration.

It demonstrates how Lean Six Sigma tools can help reduce **picking errors**, **stockouts**, and **inefficiencies** in warehouse operations using accessible tools like Excel.

---

## Objective

Reduce operational waste and improve performance by:
- Minimizing picking errors
- Reducing stockout incidents
- Optimizing picking time and inventory control
- Establishing a repeatable, data-driven control plan

---

## Project Structure
lean-six-sigma-warehouse-dashboard/
├── data/
│ └── warehouse_inventory_dataset_30000.xlsx # Cleaned dataset (30,000 rows)
├── analysis/
│ └── excel_kpis_summary.xlsx # Excel file with KPIs and pivot tables
├── docs/
│ ├── dmaic_report.md # Full DMAIC project documentation
│ └── column_descriptions.md # Column-level data dictionary
└── README.md # Project overview


---

## Methodology – DMAIC

| Phase    | Description |
|----------|-------------|
| **Define**   | Identified high error rate, stockouts, and variability in lead time |
| **Measure**  | Calculated KPIs using Excel (e.g., picking error rate, stockout rate, lead time) |
| **Analyze**  | Root causes identified using segmentation and Pareto analysis |
| **Improve**  | Layout redesign, picker training, smarter reorder point logic |
| **Control**  | Excel-based control dashboard tracks KPIs over time |

Full report: [`docs/dmaic_report.md`](docs/dmaic_report.md)

---

## Dataset

- **Rows:** 30,000 simulated warehouse transactions  
- **Generated:** Synthetically, for educational and portfolio purposes  
- **Key Fields:**
  - Order metadata: `Order ID`, `Order Date`, `Region`, `SKU`
  - Process metrics: `Units Ordered`, `Units Shipped`, `Picking Time`, `Lead Time`
  - Inventory metrics: `Inventory Level`, `Reorder Point`, `Stockout`, `Order Accuracy (%)`

Column descriptions: [`docs/column_descriptions.md`](docs/column_descriptions.md)

---

## Key Outcomes (Simulated)

| Metric                | Before     | After       | Change    |
|-----------------------|------------|-------------|-----------|
| Picking Error Rate    | 10.5%      | **8.58%**    | ↓ 18%     |
| Stockout Rate         | 32.5%      | **25.32%**   | ↓ 22%     |
| Order Accuracy        | 89%        | **91.42%**   | ↑ 2.7%    |
| Lead Time             | 6.2 days   | **5.51 days**| ↓ 11%     |

---

## How to Use

1. Open the Excel file: `analysis/excel_kpis_summary.xlsx`
   - Review KPI calculations, pivot tables, and root cause analysis
2. Read the report:
   - Explore each phase of the DMAIC process in `docs/dmaic_report.md`

---

## Disclaimer

This project uses **synthetic data** and is intended for **educational and portfolio use only**.  
It does **not** represent actual warehouse operations or real customer data.

---

## License

This project is licensed under the **MIT License**.  
You are free to use, modify, and distribute this project for personal or commercial purposes, as long as you include the original license and attribution.

See the full license text in the [`LICENSE`](LICENSE) file.
