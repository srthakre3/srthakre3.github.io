## Architecture

![Analytics Platform Architecture](docs/architecture.svg)

Raw e-commerce data flows through Redshift into dbt's three-layer transformation model (staging → intermediate → mart), feeds a governed metric layer (revenue, churn, cohort), and surfaces in interactive QuickSight/Tableau dashboards. The star schema centers on `fact_orders` with dimension tables for customers, products, dates, and channels.
