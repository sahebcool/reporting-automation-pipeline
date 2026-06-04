# Reporting Automation Pipeline

**Author:** Amit Choudhury  
**Tools:** Python · pandas · NumPy · matplotlib  
**Domain:** Data Engineering | ETL | Reporting Automation

---

## 📌 Project Overview

Automates 4 manual reporting workflows — Sales, SLA Compliance, Operations, and Finance — reducing a 3-hour manual process to a ~12-minute scheduled run. Generates 4 analysis-ready datasets and 4 dashboard reports automatically.

---

## ⚡ Impact

| Metric | Before | After |
|--------|--------|-------|
| Report generation time | ~3 hours | ~12 minutes |
| Delivery to business teams | 2–3 days | Same day |
| Manual effort per week | 8+ hours | Near zero |
| Datasets generated/month | Ad hoc | 10+ structured CSVs |

---

## 📁 Project Structure

```
project2_automation_pipeline/
│
├── pipeline.py                     # Main automation script
│
├── raw_sources/                    # Extracted raw data (auto-generated)
│   ├── sales_transactions.csv
│   ├── sla_compliance.csv
│   ├── operational_metrics.csv
│   └── finance_summary.csv
│
├── cleaned_reports/                # Analysis-ready cleaned datasets
│   ├── sales_clean.csv
│   ├── sla_clean.csv
│   ├── ops_clean.csv
│   └── finance_clean.csv
│
└── visuals/                        # Auto-generated report images
    ├── report1_sales_performance.png
    ├── report2_sla_compliance.png
    ├── report3_operations.png
    ├── report4_finance.png
    └── pipeline_architecture.png
```

---

## 🚀 How to Run

```bash
# Step 1: Install dependencies
pip install pandas numpy matplotlib

# Step 2: Run the full pipeline
python pipeline.py
```

All 4 reports and cleaned datasets are generated automatically in one run.

---

## 🔄 Pipeline Architecture

```
[ EXTRACT ]  →  [ CLEAN ]  →  [ TRANSFORM ]  →  [ REPORT ]
4 sources       Null handling   Feature eng.      4 dashboards
2,500–10,000    Validation      KPI calculation   Same-day
rows each       Deduplication   Aggregation       delivery
```

---

## 📊 What Each Report Covers

| Report | Key Metrics |
|--------|-------------|
| **Sales Performance** | Revenue by region, product, rep; monthly trend; transaction status |
| **SLA Compliance** | SLA met % by team & priority; monthly trend; breach highlighting |
| **Operational Metrics** | Throughput, error rate, productivity index, system availability |
| **Finance Summary** | Budget vs actual, variance %, cost per headcount trend |

---

## 🛠️ Skills Demonstrated

- `pandas` — multi-source data extraction, cleaning, transformation, aggregation
- `NumPy` — numerical computations, data simulation
- `matplotlib` — automated chart and dashboard generation
- ETL pipeline design — modular extract → clean → transform → report flow
- Scheduling-ready architecture — script can be run via cron job or task scheduler
