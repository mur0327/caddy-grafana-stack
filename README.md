# Caddy with Grafana + Alloy + Prometheus + Loki

## Folder Structure

```
📦 caddy-grafana-stack
├─ caddy
│  ├─ config
│  ├─ data
│  ├─ logs
│  ├─ srv
│  ├─ Caddyfile
│  └─ compose.yml
└─ grafana
   ├─ config
   │  ├─ alloy
   │  │  └─ config.alloy
   │  ├─ grafana
   │  │  ├─ datasources
   │  │  │  └─ datasource.yml
   │  │  └─ grafana.ini
   │  └─ prometheus
   │     └─ prometheus.yml
   └─ compose.yml
```

## Usage

### Git Clone
```bash
git clone https://github.com/mur0327/caddy-grafana-stack.git
```

### Create Docker Network
```bash
docker network create docker
```

### Caddy
```bash
cd caddy

docker compose up -d
```

### Grafana Stack
```bash
cd grafana-stack

docker compose up -d
```
