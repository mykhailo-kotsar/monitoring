# Monitoring Stack

Production-ready monitoring setup using Prometheus + Grafana + Node Exporter with Telegram alerting.

## Components

- **Prometheus** — metrics collection (port 9090)
- **Grafana** — visualization and dashboards (port 3000)
- **Node Exporter** — system metrics (CPU, RAM, Disk, Network)
- **Telegram alerts** — notifications when thresholds exceeded

## Quick Start

```bash
git clone https://github.com/mykhailo-kotsar/monitoring
cd monitoring
```

Edit `provisioning/alerting/telegram.yml` — add your bot token and chat ID.

```bash
docker-compose up -d
```

Open Grafana: `http://YOUR_IP:3000`
- Login: admin
- Password: set via GF_SECURITY_ADMIN_PASSWORD in docker-compose.yml
- Import dashboard ID: `1860`

## Alerts

- **High Memory Usage** — triggers when available RAM drops below 100MB
- Notifications delivered to Telegram

## Stack
Docker · docker-compose · Prometheus · Grafana · Node Exporter · Telegram Bot API
