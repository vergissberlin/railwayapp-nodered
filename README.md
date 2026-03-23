# Node-RED

![Template Header](./template-header.svg)


Deploy Node-RED on Railway with one click.

[![Deploy on Railway](https://railway.com/button.svg)](https://railway.com/deploy/56bdr8?referralCode=2_sIT9&utm_medium=integration&utm_source=template&utm_campaign=generic)

## ✨ Features

* Node-RED accessible on HTTPS
* Password Authentication (Set username & password in environment variables)
* FlowFuse Dashboard via `@flowfuse/node-red-dashboard`
* Railway config as code via `railway.toml`

## Production recommendations (Railway)

* Keep credentials in Railway Variables, never in `.env` committed to Git
* Use the built-in healthcheck endpoint at `/healthz` (configured in `railway.toml`)
* Use a persistent volume for Node-RED data in production

## 🚀 How to Deploy

1. Click Deploy on Railway and setup your credentials

```bash
NODE_RED_CREDENTIAL_SECRET=yoursecret
NODE_RED_USERNAME=yourusername
NODE_RED_PASSWORD=yourpassword
# optional alternative to NODE_RED_PASSWORD (bcrypt hash)
NODE_RED_PASSWORD_HASH=$2a$10$...
NODE_RED_EDITOR_URI="/" # optional
NODE_RED_DASHBOARD_URI="/ui" # optional FlowFuse dashboard path
```

2. Wait for Build & Deployment to Finish
3. Login with credentials

## Persistent storage (recommended)

Node-RED stores flows and runtime state in the user directory. For production use, attach a Railway volume and mount it to `/data`.

The template uses this start command by default:

```bash
node-red -u /data --settings /app/settings.js
```

This keeps your flows and credentials persistent across redeployments.

## 🪲 Bug Reporting

If you find a bug in the template for railway, you can [submit an issue](https://github.com/vergissberlin/railwayapp-nodered/issues/new) to the GitHub Repository. Even better you can submit a Pull Request with a fix.

<!-- footer -->
<!-- footer -->
[![Airbyte](https://img.shields.io/badge/Airbyte-615EFF?style=for-the-badge&logo=airbyte&logoColor=white)](https://github.com/vergissberlin/railwayapp-airbyte)
[![Apache Airflow](https://img.shields.io/badge/Apache%20Airflow-017CEE?style=for-the-badge&logo=apacheairflow&logoColor=white)](https://github.com/vergissberlin/railwayapp-airflow)
[![CodiMD](https://img.shields.io/badge/CodiMD-0F766E?style=for-the-badge&logo=markdown&logoColor=white)](https://github.com/vergissberlin/railwayapp-codimd)
[![Email Service](https://img.shields.io/badge/Email%20Service-2563EB?style=for-the-badge&logo=maildotru&logoColor=white)](https://github.com/vergissberlin/railwayapp-email)
[![GitLab CE](https://img.shields.io/badge/GitLab%20CE-FC6D26?style=for-the-badge&logo=gitlab&logoColor=white)](https://github.com/vergissberlin/railwayapp-gitlab)
[![Grafana](https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white)](https://github.com/vergissberlin/railwayapp-grafana)
[![Home Assistant](https://img.shields.io/badge/Home%20Assistant-18BCF2?style=for-the-badge&logo=homeassistant&logoColor=white)](https://github.com/vergissberlin/railwayapp-homeassistant)
[![InfluxDB](https://img.shields.io/badge/InfluxDB-22ADF6?style=for-the-badge&logo=influxdb&logoColor=white)](https://github.com/vergissberlin/railwayapp-influxdb)
[![Mosquitto MQTT](https://img.shields.io/badge/Mosquitto%20MQTT-3C5280?style=for-the-badge&logo=eclipsemosquitto&logoColor=white)](https://github.com/vergissberlin/railwayapp-mqtt)
[![Node-RED](https://img.shields.io/badge/Node--RED-8F0000?style=for-the-badge&logo=nodered&logoColor=white)](https://github.com/vergissberlin/railwayapp-nodered)
[![OpenSearch](https://img.shields.io/badge/OpenSearch-005EB8?style=for-the-badge&logo=opensearch&logoColor=white)](https://github.com/vergissberlin/railwayapp-opensearch)
[![TYPO3 CMS](https://img.shields.io/badge/TYPO3%20CMS-FF8700?style=for-the-badge&logo=typo3&logoColor=white)](https://github.com/vergissberlin/railwayapp-typo3)
