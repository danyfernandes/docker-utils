# docker-utils

This repository contains configurations and setup scripts for managing Docker containers for various services and monitoring stacks.

## Contents

- `airflow/`: Docker Compose setup and configurations for Airflow.
- `debezium/`: Docker Compose setup and configurations for Debezium with RabbitMQ.
- `monitoring/`: Docker Compose setup and configurations for monitoring services.
- `README.md`: docker-utils repository README file.

## Services

- **Airflow Stack**: Includes PostgreSQL, Airflow-Webserver, Airflow-Triggerer, Airflow-Init and Airflow-Cli.
- **Debezium Stack**: Includes Debezium.
- **Monitoring Stack**: Includes RabbitMQ, NodeExporter, cAdvisor, Prometheus, Grafana, Promtail, Loki, and Portainer.

## Usage

- [Airflow Services README](airflow/README.md) for Airflow services setup instructions.
- [Debezium Services README](debezium/README.md) for Debezium services setup instructions.
- [Monitoring Setup README](monitoring/README.md) for monitoring setup instructions.

For detailed information, navigate to the respective directories and view their README files.
