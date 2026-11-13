# Trading Journal

Ein Trading-Tagebuch in Kalenderform – eine einzelne HTML-Datei ohne Build-Schritt.

- **Kalender**: Jeder Tag zeigt P&L und Anzahl der Trades (grün/rot), dazu Wochensummen und Monatskennzahlen (Trefferquote, Profit-Faktor, bester/schlechtester Tag).
- **Tagesansicht**: Klick auf einen Tag zeigt alle Trades mit Einstieg, Ausstieg, Menge, R-Multiple, Setup, Notizen und der damals abgehakten Checkliste. Trades lassen sich bearbeiten und löschen.
- **Checkliste**: Unter „Checkliste“ legst du deine eigenen Regeln an. Bei jedem neuen Trade wird sie zuerst abgefragt; fehlende Punkte werden markiert und in der Statistik „Checklisten-Disziplin“ ausgewertet (P&L mit vs. ohne vollständige Checkliste).

## Starten

`index.html` im Browser öffnen. Die Daten werden im `localStorage` des Browsers gespeichert.
Als claude.ai-Artifact veröffentlicht, speichert die App zusätzlich privat pro Nutzer in der Artifact-Datenbank und synchronisiert zwischen Geräten.

## Als App aufs Handy

Die App ist eine **Progressive Web App (PWA)**: installierbar, offline nutzbar, mit eigenem Icon und ohne Browserleiste.

1. **Online stellen (einmalig):** Branch nach `main` mergen, dann im Repo unter *Settings → Pages → Build and deployment → Source* „**GitHub Actions**“ wählen. Der Workflow `.github/workflows/pages.yml` veröffentlicht die App unter `https://<benutzer>.github.io/trade/`.
2. **Installieren:**
   - **iPhone (Safari):** Seite öffnen → Teilen-Symbol → „Zum Home-Bildschirm“.
   - **Android (Chrome):** Seite öffnen → Menü ⋮ → „App installieren“ bzw. „Zum Startbildschirm hinzufügen“.

Die Daten liegen lokal auf dem Gerät. Unter *Checkliste → Daten sichern* kannst du ein Backup (JSON) exportieren und wieder importieren, z. B. für einen Handywechsel.
