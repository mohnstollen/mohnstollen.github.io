# Apps

Übersichtsseite im Stil eines App Stores: https://mohnstollen.github.io/

Alle Apps mit Icon, Screenshots, Beschreibung und Download (APK aus dem neuesten GitHub-Release bzw.
Link zur Web-App). Die Seite ist eine einzelne `index.html` ohne Build-Schritt und ohne Abhängigkeiten.

## App hinzufügen oder ändern
- Eintrag in der Liste `APPS` oben im Skript von `index.html`
- Icon als `icons/<id>.png`
- Screenshots als `screenshots/<id>-1.webp`, `-2.webp` … (Hochformat 360 × 740, die Anzahl steht im
  Eintrag unter `shots`)

Version, Datum und Größe einer APK holt die Seite beim Öffnen aus dem neuesten Release des jeweiligen Repos.

## Veröffentlichen
GitHub Pages: Settings → Pages → Source „Deploy from a branch“, Branch `main`, Ordner `/ (root)`.
Jeder Push auf `main` aktualisiert die Seite.

## Lokal ansehen
```bash
python3 -m http.server 8000   # dann http://localhost:8000
```
