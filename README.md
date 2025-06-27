# Realtime Data Streaming | End-to-End Data Engineering Project

## Introduction

This project demonstrates building a data processing pipeline using modern technologies. The work uses Apache Airflow for task orchestration, Kafka and Zookeeper for streaming data, Spark for distributed processing, and Cassandra as a storage. All components are deployed in Docker containers, which ensures convenient management and scaling of the system.

## System Architecture

![System Architecture](https://github.com/igor-ml-2007/data-streaming/blob/main/data-streaming-pipeline/project_architecture.png)

The project is designed with the following components:

- **Data Source**: We use `randomuser.me` API to generate random user data for our pipeline.
- **Apache Airflow**: Responsible for orchestrating the pipeline and storing fetched data in a PostgreSQL database.
- **Apache Kafka and Zookeeper**: Used for streaming data from PostgreSQL to the processing engine.
- **Control Center and Schema Registry**: Helps in monitoring and schema management of our Kafka streams.
- **Apache Spark**: For data processing with its master and worker nodes.
- **Cassandra**: Where the processed data will be stored.


## Technologies

- Apache Airflow
- Python
- Apache Kafka
- Apache Zookeeper
- Apache Spark
- Cassandra
- PostgreSQL
- Docker

## Getting Started

1. Clone the repository:
    ```bash
    git clone https://github.com/igor-ml-2007/data-streaming
    ```

2. Navigate to the project directory:
    ```bash
    cd data-streaming-pipeline
    ```

3. Downloading all the necessary packages for project:
    ```bash
    pip install -r requirements.txt
    ```
4. Run Docker Compose to spin up the services:
    ```bash
    docker-compose up
    ```



