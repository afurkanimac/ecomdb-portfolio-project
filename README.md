## Project Overview
Modern e-commerce companies require fast, reliable, and scalable data systems. This project simulates the architecture of a retail/e-commerce platform using a combination of:

- **MySQL (OLTP order & customer transactions)**
- **PostgreSQL (analytics + partitioned tables + replication)**
- **MongoDB (product catalog & event store)**
- **Airflow, Kafka, Spark (ETL & streaming pipelines)**
- **Prometheus + Grafana (monitoring)**
- **Backup & Restore scripts**
- **K6 & JMeter (load testing)**

This repository reflects the responsibilities of a **Database Administrator** working in a high-traffic retail company.

---

## 📁 Repository Structure
```
ecomdb-portfolio-project/
│
├── 1-relational-databases/
│   ├── mysql/
│   │   ├── schema.sql
│   │   ├── indexes.sql
│   │   ├── sample-data.sql
│   │   └── procedures/
│   └── postgresql/
│       ├── schema.sql
│       ├── partitioning.sql
│       ├── replication-setup.md
│       └── sample-data.sql
│
├── 2-nosql/
│   ├── mongo/
│       ├── products.json
│       ├── customers.json
│       └── orderEvents.json
│
├── 3-etl-and-data-pipelines/
│   ├── airflow/
│   │   ├── dag_etl_orders.py
│   │   └── dag_daily_backup.py
│   ├── kafka/
│   │   └── create-topics.sh
│   └── spark/
│       └── transform_orders.py
│
├── 4-admin-operations/
│   ├── backup/
│   │   ├── mysql-backup.sh
│   │   ├── postgres-backup.sh
│   │   └── mongo-backup.sh
│   ├── monitoring/
│   │   ├── grafana-dashboards.json
│   │   └── prometheus-rules.yml
│   └── runbooks/
│       ├── replication-failure.md
│       ├── slow-query.md
│       ├── disk-usage.md
│       └── high-cpu.md
│
├── 5-load-testing/
│   ├── k6-script.js
│   └── jmeter-testplan.jmx

```

---

## 🎯 Project Goals

### **1. Database Design & Architecture**
- Normalized OLTP schema design
- PostgreSQL partitioning for large fact tables
- MongoDB schema modeling for product catalogs
- Replication + failover strategies

### **2. Database Administration**
- User management & permissions
- Backup/restore flows
- Disaster recovery runbooks
- Indexing strategy & query optimization
- Monitoring (Prometheus/Grafana)

### **3. Data Engineering**
- Airflow DAGs for ETL
- Kafka topics for event-driven systems
- Spark jobs for transformation

### **4. Performance Engineering**
- K6 load test for checkout API
- JMeter test plan for order flows
- Slow query troubleshooting

---

## 🗂️ Use Cases Covered
This project simulates real e-commerce operations:

### ✔ Order placement
### ✔ Payment events
### ✔ Inventory updates
### ✔ Product catalog browsing
### ✔ Customer management
### ✔ Real-time event logging
### ✔ Daily ETL for analytics
### ✔ Automated backups
### ✔ Database monitoring dashboards

---

## 📦 Technologies Used
**Databases**: MySQL, PostgreSQL, MongoDB  
**Pipelines**: Airflow, Kafka, Spark  
**Monitoring**: Prometheus, Grafana  
**Load Testing**: K6, JMeter  
**DevOps Tools**: Bash, Docker (optional), Git

---

## 📌 How to Use This Repository
1. Clone the repo:  
   ```bash
   git clone https://github.com/afurkanimac/ecomdb-portfolio-project.git
   ```

2. Review the architecture (`1-architecture/`)

3. Set up MySQL, PostgreSQL, MongoDB schemas using files in `2-relational-databases/` and `3-nosql/`

4. Execute ETL jobs using Airflow / Spark configuration

5. Explore DBA scripts in `5-admin-operations/`

6. Run load tests in `6-load-testing/`

---

Contributions, suggestions, and improvements are welcome!
For collaboration or inquiries, feel free to reach out via LinkedIn.



## ⭐ Support
If you find this project helpful, please consider starring the repository!
