# Deployment & Operations Guide: Custom Chart

## 🚀 Live Access URLs
- **Public Preview URL:** [https://river-alternatives-isolated-parker.trycloudflare.com/preview/prod-custom-chart-5ca927/](https://river-alternatives-isolated-parker.trycloudflare.com/preview/prod-custom-chart-5ca927/)
- **Local Gateway Path:** [/preview/prod-custom-chart-5ca927/](/preview/prod-custom-chart-5ca927/)
- **Internal Port:** `8109`
- **Process PID:** `587768`
- **Runtime Engine:** `python_preview`
- **Health Status:** `HEALTHY (HTTP 200)`
- **Deployed Timestamp:** `2026-09-19T19:06:10.605211+00:00`

## 📋 Execution Command
```bash
/usr/local/lib/hermes-agent/venv/bin/python3 app.py --port 8109
```

## 🩺 Health Check Verification
```bash
curl -I http://127.0.0.1:8109/
```

## 📜 Live Deployment Logs
Logs are stored at `/tmp/pytest-of-root/pytest-13/test_backlog_engine_product_sc0/custom_prod_ws/logs/deploy.log`.
