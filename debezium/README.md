# Debezium

This directory contains Docker Compose setup and configurations for Debezium service:

## Services

- **Debezium**: Debezium is an open source distributed platform for change data capture.

## Contents

- `docker-compose.yml`: Docker Compose file defining Debezium setup.
- `conf/`: Folder containing Debezium configurations:
  - `application.properties`

## Usage

1. Navigate to the `debezium/` directory.
2. To start the Debezium stack, run:

   ```bash
   docker compose up -d
   ```

3. To stop and delete all Debezium containers, networks, and volumes, run:
    
    ```bash
   docker compose down
   ```