# Apache Airflow Tutorials

A collection of tutorials and example DAGs to learn Apache Airflow — a platform to programmatically author, schedule, and monitor workflows.

## 📦 Project Structure

├── dags/ # DAG definitions go here <br>
├── logs/ <br>
├── plugins/ <br>
├── docker-compose.yaml # Docker Compose setup for Airflow <br>
├── .env # Environment variables <br>
└── README.md <br>



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


To create a user in the apache airflow server use this command for example:

```bash
airflow users create --username admin --firstname firstname --lastname lastname --role Admin --email admin@admin.com
```
