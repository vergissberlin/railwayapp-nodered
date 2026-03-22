# Agent Guide

## Projektueberblick
- Dieses Repository ist ein schlankes Node-RED-Template fuer Railway.
- Ziel: Node-RED schnell deployen, ueber HTTPS bereitstellen und den Editor per Umgebungsvariablen absichern.
- Der eigentliche Flow-Inhalt liegt in `flows.json` (aktuell leer: `[]`).

## Tech-Stack
- Runtime: Node.js
- Kernpaket: `node-red` (~3.x.x)
- Zusatzpakete: `node-red-dashboard`, `node-red-contrib-ngrok`, `when`
- Konfiguration: `settings.js` (Node-RED Runtime-Konfig)

## Wichtige Dateien
- `package.json`: Startskripte und Abhaengigkeiten
- `settings.js`: Sicherheit, Ports, Pfade, Runtime-Optionen
- `flows.json`: exportierte Node-RED-Flows
- `README.md`: Deploy-Dokumentation fuer Railway

## Laufverhalten
- Start (prod): `npm start` (`node-red -u .`)
- Start (dev): `npm run start:dev` (setzt Test-Credentials inline)
- Port: `process.env.PORT` oder Fallback `1880`
- Editor-Route: `NODE_RED_EDITOR_URI` (Default `/`)
- Dashboard-Route: `NODE_RED_DASHBOARD_URI` (Default `ui`)

## Erforderliche Umgebungsvariablen
- `NODE_RED_CREDENTIAL_SECRET`
- `NODE_RED_USERNAME`
- `NODE_RED_PASSWORD`
- Optional:
  - `NODE_RED_EDITOR_URI`
  - `NODE_RED_DASHBOARD_URI`

## Sicherheitsnotizen
- `adminAuth` vergleicht Username/Passwort direkt gegen Umgebungsvariablen.
- Damit wird kein gehashter Passwortspeicher genutzt; fuer ein produktives Hardening waere bcrypt-basierte Validierung sinnvoll.
- Keine Secrets in `flows.json` oder ins Repository committen.

## Aktueller Status
- Das Projekt ist als Deployment-Template vorbereitet.
- Es existieren noch keine konkreten Flows oder automatisierte Tests.

## Arbeitskonvention fuer Agents
- Bei Funktionsaenderungen zuerst `settings.js` und `README.md` auf Konsistenz pruefen.
- Neue Features moeglichst ueber Umgebungsvariablen steuerbar machen.
- Bei Aenderungen an Startverhalten oder Pfaden immer Doku in `README.md` mit aktualisieren.
