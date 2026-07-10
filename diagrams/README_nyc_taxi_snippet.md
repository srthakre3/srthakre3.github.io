## Architecture

![ELT Pipeline Architecture](docs/architecture.svg)

The pipeline ingests raw NYC TLC trip data via Python into PostgreSQL, transforms it with dbt across three layers (staging → intermediate → dimensional mart with a star schema), orchestrates the full workflow with Apache Airflow DAGs, and enforces data quality with 22 dbt tests and a CI/CD pipeline on GitHub Actions.
