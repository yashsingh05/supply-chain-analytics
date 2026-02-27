# Supply Chain Analytics Dashboard

## Overview
An end-to-end supply chain analysis project identifying stockout risks, supplier performance, and reorder priorities across 100 SKUs using Python, SQL, and Power BI.

## Business Problem
Which products are at risk of running out of stock? Which suppliers are underperforming? Where should we prioritize reorders?

## Approach
- **Data:** Kaggle Supply Chain Dataset (100 SKUs, 5 suppliers, 3 product categories)
- **Feature Engineering:** Daily demand rate, days of supply, stockout risk flags, reorder quantities
- **SQL Analysis:** Revenue by product type, stockout risk by supplier, top at-risk SKUs, shipping cost by carrier
- **Dashboard:** Interactive Power BI report with product type slicer and KPI cards

## Key Findings
| Insight | Value |
|---------|-------|
| SKUs at stockout risk | 81 out of 100 (81%) |
| Total revenue | $577.60K |
| Avg days of supply | 6.5 days |
| Worst supplier | Supplier 3 (avg 3.1 days of supply) |
| Top revenue category | Skincare ($241K) |

## Recommended Actions
- **Immediate reorder** for SKU34, SKU68 — already at 0 days of supply
- **Audit Supplier 3** — lowest avg days of supply across all suppliers
- **Use Carrier B** for urgent shipments — cheapest and fastest carrier

## Tools Used
- Python (Pandas, NumPy, Matplotlib, Seaborn)
- SQLite + SQLAlchemy
- Jupyter Notebook
- Power BI Desktop

## Files
- `supply_chain.ipynb` — Full Python + SQL pipeline
- `supply_chain_clean.csv` — Cleaned dataset with engineered features
- `Supply_Chain_Dashboard.pbix` — Power BI dashboard
- `supply_chain_viz.png` — Python visualizations
