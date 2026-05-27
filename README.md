# Hi, I'm Vladyslav 👋

Backend / Full-Stack Developer with experience in building
and maintaining production systems. Strong focus on database performance,
data pipelines, and maintainable backend architectures.

## 🔧 Tech Stack
- Python
- Django, FastAPI
- PostgreSQL, SQLAlchemy
- HTMX
- Docker, GitLab
- Kafka, Airflow
- MinIO

## 🎯 Core Focus
- Database performance and query optimization
- Refactoring and evolving production schemas
- Data pipelines and event-driven architectures
- Maintainable and readable backend code
- Service-layer architecture and clean design

## 📂 Selected Projects

### 🔹 Medallion ETL Pipeline
🔗 **Repository:** *https://github.com/dema-git/data-flow*

Event-driven data pipeline where synthetic user sessions are generated, streamed through Kafka, 
stored in object storage, transformed, and finally loaded into PostgreSQL 
via Airflow-orchestrated workflows.

**Key components:**
- Synthetic session generator
- Kafka for event streaming
- MinIO for batch storage
- Airflow DAGs invoking backend services via API
- PostgreSQL as the final analytical store

**Tech:**  
`Python · FastAPI · Kafka · Airflow · MinIO · PostgreSQL`

---

### 🔹 AI Data Quality Ops
🔗 **Repository:** *https://github.com/dema-git/ai-data-quality-ops*

Data quality operations layer built on top of a Medallion ETL pipeline.  
It adds controlled bad-data generation, deterministic validation, quarantine reports, 
incident routing, and optional OpenAI-based explanations for detected data-quality issues.

**Key components:**
- Controlled bad-data injection
- Deterministic validation before Silver processing
- Quarantine bucket for rejected records
- Quality issue summary and incident reports
- Rule-based routing to specialist incident profiles
- Mock/OpenAI modes for incident explanation
- Dashboard with quality metrics and AI-generated analysis

**Tech:**  
`Python · FastAPI · Kafka · Airflow · MinIO · PostgreSQL · OpenAI API`

---

### 🔹 Zero-Downtime Database Migrations
🔗 **Repository:** *https://github.com/dema-git/cdc-zero-downtime-migration*  

Research and implementation of safe database schema evolution strategies
without service downtime. Focused on refactoring large production tables
into smaller, more maintainable structures.

**Key components:**
- Parallel old/new schemas
- Dual writes via Kafka
- Batch backfilling of historical data
- WAL / CDC-based consistency
- Gradual read-switch strategy

**Tech:**  
`PostgreSQL · Kafka · Python · WAL / CDC concepts · Debezium · Grafana`

---

## 🛠 Engineering Practices
- Clear separation between API, service, and data layers
- Performance-aware SQL queries
- Defensive programming and structured error handling
- Refactoring legacy systems safely in production
- Writing maintainable and readable code

## 📫 Contact
Email: demenkov.dev@gmail.com  
LinkedIn: https://www.linkedin.com/in/vladyslav-demenkov-84167226a/
