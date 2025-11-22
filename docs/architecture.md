# Architecture

This document describes the high-level architecture of the Real Estate Lakehouse.

Pipeline:
- Scrapers collect raw HTML / JSON
- Raw data stored in MinIO (S3-compatible)
- Delta Lake Bronze: raw ingested data
- Delta Lake Silver: cleaned/normalized (CDC applied)
- Delta Lake Gold: aggregated tables for analytics
- Dagster orchestrates jobs
- Superset / Notebooks for analytics and dashboards
