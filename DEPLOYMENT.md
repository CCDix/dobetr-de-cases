# Deployment auf GitHub

## Vorbereitung

Diese Repository ist für GitHub Pages optimiert und wird automatisch gehostet.

### Anforderungen
- GitHub Account
- Git installiert
- SSH oder HTTPS Zugang konfiguriert

---

## Schritt 1: Repository auf GitHub erstellen

1. Gehe zu https://github.com/new
2. Erstelle ein neues Repository mit dem Namen: `dobetr-de-cases`
3. **Wichtig:** Setze es auf **Public** (für GitHub Pages)
4. Initialisiere NICHT mit README (wird ohnehin hochgeladen)

---

## Schritt 2: Lokales Git-Setup

```bash
cd /pfad/zu/dobetr-de-cases

# Git initialisieren
git init

# Remote hinzufügen (ersetze USERNAME mit deinem GitHub-Benutzernamen)
git remote add origin https://github.com/CCDix/dobetr-de-cases.git

# Branch umbenennen zu main
git branch -M main
```

---

## Schritt 3: Commits und Push

```bash
# Alle Dateien hinzufügen
git add .

# Ersten Commit erstellen
git commit -m "Initial commit: Case study portal für PACE assessments 2026"

# Zum GitHub pushen
git push -u origin main
```

---

## Schritt 4: GitHub Pages aktivieren

1. Gehe zum Repository auf GitHub: https://github.com/CCDix/dobetr-de-cases
2. Klicke auf **Settings**
3. Navigiere zu **Pages** (linke Sidebar)
4. Unter "Source" wähle **Deploy from a branch**
5. Wähle Branch: **main**
6. Wähle Folder: **/ (root)**
7. Klicke **Save**

---

## Schritt 5: Custom Domain konfigurieren (Optional)

Falls du `cases.dobetr.de` verwenden möchtest:

1. Gehe zu **Settings** → **Pages**
2. Unter "Custom domain" gib `cases.dobetr.de` ein
3. Klicke **Save**
4. Konfiguriere DNS bei deinem Hosting-Provider:
   - Wende dich an deinen DNS-Provider
   - Erstelle einen CNAME-Record:
     ```
     Name: cases
     Type: CNAME
     Value: CCDix.github.io
     ```

---

## Verifizierung

Nach 1–5 Minuten sollte die Website verfügbar sein:
- Ohne Custom Domain: https://CCDix.github.io/dobetr-de-cases/
- Mit Custom Domain: https://cases.dobetr.de

---

## Updates durchführen

Nach Änderungen lokal:

```bash
git add .
git commit -m "Beschreibung der Änderung"
git push origin main
```

Die Website wird automatisch aktualisiert (innerhalb von 1 Minute).

---

## Struktur

```
dobetr-de-cases/
├── index.html           # Hauptseite
├── 404.html             # Error Page
├── styles.css           # Styling (dobetr.de Design)
├── README.md            # Dokumentation
├── DEPLOYMENT.md        # Diese Datei
├── CNAME                # Custom Domain
├── _config.yml          # GitHub Pages Config
├── .gitignore           # Git Ignore
└── assets/
    └── logos/
        └── README.md    # Logo-Platzhalter & Instruktionen
```

---

## Troubleshooting

### Website wird nicht angezeigt
- Warte 5 Minuten nach dem Push
- Prüfe Settings → Pages → Deployment Status

### Custom Domain funktioniert nicht
- Überprüfe DNS-Records (kann 24h dauern)
- Stelle sicher, dass CNAME-Datei im Root ist

### Styling wird nicht geladen
- Prüfe, dass `styles.css` im Root-Verzeichnis ist
- Browser-Cache leeren (Ctrl+Shift+Del)

---

## Support

📧 hello@dobetr.de

