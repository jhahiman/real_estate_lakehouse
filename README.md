# Real Estate Lakehouse Platform

This project builds a full end-to-end Real Estate Analytics Lakehouse using:

- **Python + BeautifulSoup** (Scraping)
- **MinIO** (S3-compatible object store)
- **Delta Lake + Spark** (Lakehouse storage + CDC)
- **Dagster** (Orchestration)
- **Apache Superset** (Dashboards)
- **Docker Compose** (Local reproducible platform)
- **Databricks Free Edition** (Cloud-scale Delta Lake & ML)

## Architecture Overview
End-to-end pipeline:
Scraper → MinIO Raw Layer → Delta Bronze → Delta Silver (CDC) → Gold → Dagster → Superset → Notebooks / Databricks

## Folder Structure
```text
REAL_ESTATE_LAKEHOUSE/
│
├── infra/
│   ├── docker-compose.yml
│   └── README.md
│
├── src/
│   ├── ingestion/
│   │   └── scraper/
│   ├── pipelines/
│   │   └── spark_jobs/
│   └── cdc/
│
├── orchestration/
│   └── dagster/
│
├── notebooks/
│
├── dashboards/
│
├── docs/
│   └── architecture.md
│
├── .gitignore
├── README.md
└── requirements.txt
```
