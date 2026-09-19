# Deployment & Operations Guide: Custom Chart

## 🚀 Live Access & URLs
- **Live Public Access URL:** [/preview/prod-custom-chart-5ca927/](/preview/prod-custom-chart-5ca927/)
- **Internal Port:** `0`
- **Runtime Engine:** `python_preview`
- **Deployment Status:** `DEPLOYED / ACTIVE`
- **Timestamp:** `2026-09-19T19:06:06.447140+00:00`

## 🛠️ Management & Service Control
### Launch Command
```bash
python3 app.py --port 0
```

### Health Check Probe
```bash
curl -I http://127.0.0.1:0/
```

### Systemd Service Template
```ini
[Unit]
Description=Custom Chart Service
After=network.target

[Service]
Type=simple
WorkingDirectory=/tmp/pytest-of-root/pytest-13/test_backlog_engine_product_sc0/custom_prod_ws
ExecStart=/usr/bin/python3 /tmp/pytest-of-root/pytest-13/test_backlog_engine_product_sc0/custom_prod_ws/app.py
Restart=always
RestartSec=3

[Install]
WantedBy=multi-user.target
```

## 🔒 Production Security Protocols
- HTTP-only reverse proxy via Nexus Gateway.
- Dedicated port allocation with zero port conflict.
