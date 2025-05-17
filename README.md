# Apache Airflow Tutorials

A collection of tutorials and example DAGs to learn Apache Airflow — a platform to programmatically author, schedule, and monitor workflows.

## 📦 Project Structure

├── dags/ # DAG definitions go here
├── logs/
├── plugins/
├── docker-compose.yaml # Docker Compose setup for Airflow
├── .env # Environment variables 
└── README.md



## 🚀 Getting Started

These tutorials use **Docker** and **Docker Compose** to run Apache Airflow locally.

### Prerequisites

- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/)

### 1. Clone the Repository

```bash
git clone https://github.com/GalkaKG/apache-airflow-tutorials.git
cd apache-airflow-tutorials
```

### 2. Initialize the Airflow Environment
Before the first run, initialize the database and create necessary folders:
```bash
docker-compose up airflow-init
```

This will:

- Set up the Airflow metadata database  
- Create necessary volumes and folders

### 3. Start All Airflow Services

```bash
docker-compose up
```

You can access:

- Airflow Web UI: http://localhost:8080

- Username: airflow

- Password: airflow