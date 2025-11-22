# Real Estate Lakehouse


A real estate lakehouse prototype.

Repository layout:

REAL_ESTATE_LAKEHOUSE/
├── infra/ - deployment and docker compose
├── src/ - source code (ingestion, pipelines, cdc)
├── orchestration/ - DAGs and orchestration configs
├── notebooks/ - exploratory notebooks
├── dashboards/ - dashboard assets
├── docs/ - architecture and design docs

Quick start:
1. Review `infra/docker-compose.yml` and adjust services/ports as needed.
2. Install Python dependencies from `requirements.txt`.
