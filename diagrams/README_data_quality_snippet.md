## Architecture

![Data Quality Framework Architecture](docs/architecture.svg)

The framework extracts raw tables from PostgreSQL, runs three categories of automated checks (schema validation, null/duplicate detection, statistical outlier alerting), outputs HTML and JSON reports, and enforces quality gates via pytest and GitHub Actions CI. All 6/6 tests pass.
