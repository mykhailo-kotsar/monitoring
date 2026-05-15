# Monitoring Stack

Production-ready monitoring setup using Prometheus + Grafana + Node Exporter.

## Components

- **Prometheus** — metrics collection (port 9090)
- **Grafana** — visualization and dashboards (port 3000)
- **Node Exporter** — system metrics (CPU, RAM, Disk, Network)

## Quick Start

```bash
git clone https://github.com/mykhailo-kotsar/monitoring
cd monitoring
docker-compose up -d
```

Open Grafana: `http://YOUR_IP:3000`
- Login: admin / password set via GF_SECURITY_ADMIN_PASSWORD in docker-compose.yml
- Import dashboard ID: `1860`

## Stack
Docker · docker-compose · Prometheus · Grafana · Linux
