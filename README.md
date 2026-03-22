# Node-RED

Deploy Node-RED on Railway with one click.

[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/56bdr8?referralCode=2_sIT9)

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
