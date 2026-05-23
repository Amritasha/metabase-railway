# Deploy and Host Metabase on Railway

> **Updated May 2026** — Pinned to Metabase v0.59.12 and extended healthcheck timeout for reliable deployments.

Metabase is an open-source business intelligence and data analytics platform. It lets your team explore data, build interactive dashboards, and share insights without writing SQL — connecting directly to your databases and providing an intuitive interface for data-driven decision making across the organization.

## About Hosting Metabase

Hosting Metabase requires running its Java-based application server alongside a PostgreSQL database used as its application database (storing dashboards, questions, user accounts, and settings). Metabase connects to your external data sources — such as production databases, data warehouses, or analytics stores — via JDBC drivers configured through the admin UI. On Railway, the Metabase service and its application Postgres instance are provisioned and networked automatically. The service exposes a web UI on a public Railway domain, which can be mapped to a custom subdomain for internal use.

## Common Use Cases

- Building and sharing business dashboards for revenue, product, and operations metrics
- Enabling non-technical team members to explore data without SQL knowledge
- Embedding analytics charts and dashboards into internal tools or customer-facing products

## Dependencies for Metabase Hosting

- **PostgreSQL** — application database storing Metabase configuration, dashboards, users, and query history
- **External data source** — the database or warehouse Metabase will query (e.g. your production Postgres, BigQuery, Snowflake)

### Deployment Dependencies

- [Metabase Documentation](https://www.metabase.com/docs/latest/)
- [Metabase GitHub Repository](https://github.com/metabase/metabase)
- [Metabase Self-Hosting Guide](https://www.metabase.com/docs/latest/operations-guide/running-metabase-on-docker.html)
- [Railway PostgreSQL Plugin](https://docs.railway.com/databases/postgresql)

## Why Deploy Metabase on Railway?

Railway is a singular platform to deploy your infrastructure stack. Railway will host your infrastructure so you do not have to deal with configuration, while allowing you to vertically and horizontally scale it.

By deploying Metabase on Railway, you are one step closer to supporting a complete full-stack application with minimal burden. Host your servers, databases, AI agents, and more on Railway.
