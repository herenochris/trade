# Trading Journal

Ein Trading-Tagebuch in Kalenderform – eine einzelne HTML-Datei ohne Build-Schritt.

- **Kalender**: Jeder Tag zeigt P&L und Anzahl der Trades (grün/rot), dazu Wochensummen und Monatskennzahlen (Trefferquote, Profit-Faktor, bester/schlechtester Tag).
- **Tagesansicht**: Klick auf einen Tag zeigt alle Trades mit Einstieg, Ausstieg, Menge, R-Multiple, Setup, Notizen und der damals abgehakten Checkliste. Trades lassen sich bearbeiten und löschen.
- **Checkliste**: Unter „Checkliste“ legst du deine eigenen Regeln an. Bei jedem neuen Trade wird sie zuerst abgefragt; fehlende Punkte werden markiert und in der Statistik „Checklisten-Disziplin“ ausgewertet (P&L mit vs. ohne vollständige Checkliste).

## Starten

`index.html` im Browser öffnen. Die Daten werden im `localStorage` des Browsers gespeichert.
Als claude.ai-Artifact veröffentlicht, speichert die App zusätzlich privat pro Nutzer in der Artifact-Datenbank und synchronisiert zwischen Geräten.
