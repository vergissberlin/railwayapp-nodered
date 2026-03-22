# Contributing

Danke fuer deinen Beitrag zu diesem Railway Node-RED Template.

## Ziel des Projekts
- Schnelles Deployment von Node-RED auf Railway
- Klare, einfache Konfiguration ueber Umgebungsvariablen
- Moeglichst wenig Setup-Aufwand fuer Nutzer

## Lokale Entwicklung
1. Abhaengigkeiten installieren:
   - `npm install`
2. Entwicklungsstart mit Test-Credentials:
   - `npm run start:dev`
3. Produktion aehnlich testen:
   - `npm start`

## Relevante Umgebungsvariablen
- `NODE_RED_CREDENTIAL_SECRET`
- `NODE_RED_USERNAME`
- `NODE_RED_PASSWORD`
- Optional:
  - `NODE_RED_EDITOR_URI`
  - `NODE_RED_DASHBOARD_URI`

## Beitragsrichtlinien
- Halte Aenderungen klein und fokussiert.
- Aendere nur, was fuer das jeweilige Issue/Feature noetig ist.
- Wenn sich Verhalten aendert, aktualisiere `README.md`.
- Wenn sich Runtime-Konfiguration aendert, pruefe `settings.js` sorgfaeltig auf Seiteneffekte.
- Keine Secrets, Zugangsdaten oder `.env` Inhalte committen.

## Node-RED spezifisch
- Flows liegen in `flows.json`.
- Neue Flows so bauen, dass sie auch in einer frischen Railway-Instanz funktionieren.
- Pfade (Editor/Dashboard) immer mit den konfigurierbaren Env-Variablen abgleichen.

## Pull Requests
- Beschreibe im PR kurz:
  - Was wurde geaendert?
  - Warum war die Aenderung noetig?
  - Wie kann man die Aenderung testen?
- Nutze klare, praezise Commit-Messages.

## Manuelle Checks vor PR
- App startet lokal (`npm run start:dev`).
- Login mit konfigurierten Credentials funktioniert.
- Doku ist bei Verhaltensaenderungen aktualisiert.
