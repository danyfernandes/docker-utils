# Airflow

This directory contains Docker Compose setup and configurations for Airflow services:

## Services

- **PostgreSQL**: Database backend for Airflow.
- **Airflow Webserver**: Web interface for managing Airflow DAGs and tasks.
- **Airflow Scheduler**: Component responsible for scheduling tasks.
- **Airflow Triggerer**: Handles deferred task triggers.
- **Airflow Init**: Initializes the Airflow environment.
- **Airflow CLI**: Command-line interface for Airflow.

## Contents

- `Dockerfile`: Custom Docker image configuration for Airflow.
- `requirements.txt`: Python dependencies for Airflow.
- `docker-compose.yml`: Docker Compose configuration for Airflow services.

## Usage

1. Navigate to the Airflow directory.
2. To build and initialize the environment, run:

   ```bash
   docker-compose build
   docker-compose up airflow-init
   ```

3. Start the Airflow services:

   ```bash
   docker-compose up -d
   ```

4. Access the following services through your browser:

   - Airflow Webserver: `http://localhost:8081` (default credentials: airflow/airflow)

5. To stop and delete all Airflow containers, networks, and volumes, run:

   ```bash
   docker-compose down
   ```

