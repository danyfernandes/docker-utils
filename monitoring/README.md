# Monitoring

This directory contains Docker Compose setup and configurations for monitoring services:

## Services

- **RabbitMQ**: Message broker with management UI.
- **NodeExporter**: Prometheus exporter for system metrics.
- **cAdvisor**: Container monitoring for Docker.
- **Prometheus**: Monitoring and alerting toolkit.
- **Grafana**: Metrics dashboard and graph editor.
- **Promtail**: Log collector for Loki.
- **Loki**: Log aggregation system.
- **Portainer**: Docker container management GUI.

## Contents

- `datasource.yml`: Configuration file for Grafana datasources.
- `docker-compose.yml`: Docker Compose file defining the monitoring setup.
- `grafana_dashboards/`: Folder containing Grafana dashboard configurations:
  - `docker_system_monitoring.json`
  - `node_exporter.json`
  - `rabbitmq_dashboard.json`
- `loki-config.yaml`: Configuration file for Loki log aggregation.
- `prometheus.yml`: Configuration file for Prometheus monitoring.
- `promtail-config.yaml`: Configuration file for Promtail log collector.

## Usage

1. Navigate to the `monitoring/` directory.
2. To start the monitoring stack, run:

   ```bash
   docker compose up -d
   ```

3. Access the following services through your browser:

   - Grafana: `http://localhost:3000` (default credentials: admin/admin)
   - Prometheus: `http://localhost:9090`
   - RabbitMQ Management UI: `http://localhost:15672` (default credentials: guest/guest)
   - Portainer: `http://localhost:9002` (create credentials when accessing for the first time)

4. To stop and delete all monitoring containers, networks, and volumes, run:
    
    ```bash
   docker compose down
   ```