# 🚀 Data Pipeline using DBT and Apache Airflow

## 📌 Project Overview
This project sets up an **ELT (Extract, Load, Transform) pipeline** using **DBT (Data Build Tool) and Apache Airflow**. It integrates **Postgres, Docker, and DBT** to automate data workflows, orchestrate transformations, and manage dependencies efficiently.

## ✨ Features
-  **DBT for Data Transformation**: Define models, transformations, and dependencies.
-  **Apache Airflow for Orchestration**: Automate workflow execution.
-  **PostgreSQL as Data Warehouse**: Store raw and transformed data.
-  **Docker for Containerization**: Ensures environment consistency.
-  **ELT Architecture**: Extracts, loads, and transforms data efficiently.

## 📁 File Structure
```
.
├── airflow/
│   ├── dags/
│   │   ├── elt_dag.py               # 🚀 Airflow DAG for ELT pipeline
│   │   └── airflow.cfg              # ⚙️ Airflow configuration
│   ├── custom_postgres/
│   │   ├── macros/
│   │   │   ├── film_ratings_macro.sql # 📊 SQL macros for DBT transformations
│   │   ├── models/example/
│   │   │   ├── actors.sql
│   │   │   ├── film_actors.sql
│   │   │   ├── film_ratings.sql
│   │   │   ├── films.sql
│   │   │   ├── specific_movie.sql
│   │   │   ├── schema.yml
│   │   │   ├── sources.yml
│   │   │   ├── dbt_project.yml
├── elt/
│   ├── Dockerfile                    # 🐳 Docker configuration for ELT process
│   ├── elt_script.py                  # 📝 Python script to load data from source to destination
│   ├── start.sh                        # 🚀 Shell script to initialize services
├── source_db_init/
│   ├── init.sql                        # 🎯 SQL script to initialize source database
│   ├── docker-compose.yml              # ⚙️ Docker Compose file for setting up the database
│   ├── README.md                        # 📖 Documentation for source database initialization
├── README.md                           # 📃 Project documentation
```

## ⚙️ Setup & Installation
### 📌 Prerequisites
-  Docker & Docker Compose
-  Python 3.8+
-  DBT installed
-  PostgreSQL

### 🚀 Steps to Run
1. **Clone the repository**
   ```sh
   git clone https://github.com/adityarathore622/Data-Pipeline-using-DBT-and-Apache-Airflow.git
   cd Data-Pipeline-using-DBT-and-Apache-Airflow/elt
   ```
2. **Start Docker services** 
   ```sh
   docker-compose up -d
   ```

3. **Access Airflow UI** 
   - Open `http://localhost:8080`
   - Login with credentials `admin@example.com/airflow`
4. **Trigger and Monitor DAGs** 🎯
   - Activate and trigger DAGs in the Airflow UI.

## 🚀 Future Enhancements
- 🔹 Implement CI/CD for automated deployments.
- 🔹 Add data validation and monitoring.
- 🔹 Extend support for cloud data warehouses (e.g., Snowflake, BigQuery).

## 👤 Author
**Aditya Rathore**

## 🔗 Connect with Me
- **GitHub**: [Aditya Rathore](https://github.com/adityarathore622)
- **LinkedIn**: [Aditya RAthore](https://linkedin.com/in/your-profile)

---
🌟 *Feel free to contribute or raise issues in the repository!* 


