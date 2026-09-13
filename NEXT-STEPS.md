# Nächste Schritte – dobetr.de Cases Repository

## ✅ Bereits erledigt

- [x] HTML-Struktur mit 3 Case-Studies erstellt
- [x] dobetr.de Design & Farbschema implementiert
- [x] Responsive CSS (Mobile, Tablet, Desktop)
- [x] GitHub Pages vorbereitet
- [x] README & Dokumentation
- [x] 404-Fehlerseite
- [x] Logo-Platzhalter vorbereitet

---

## 📋 Aufgaben zum Hochladen auf GitHub

### 1. **Logos hinzufügen** (Optional aber empfohlen)
Füge die offiziellen Logos in `assets/logos/` ein:
- `deutschebaseballiga.png`
- `longevity-center-nuernberg.png`
- `baumgartner-sports.png`

Dann passe `index.html` an:
```html
<div class="commissioner-logo">
    <img src="assets/logos/deutschebaseballiga.png" alt="Deutsche Baseball Liga">
</div>
```

---

### 2. **Repository auf GitHub hochladen**

```bash
cd /home/node/.openclaw/workspace/dobetr-de-cases

# Git initialisieren
git init
git remote add origin https://github.com/CCDix/dobetr-de-cases.git
git branch -M main

# Alles committen
git add .
git commit -m "Initial commit: PACE Case Studies 2026"

# Pushen
git push -u origin main
```

---

### 3. **GitHub Pages aktivieren**

1. Gehe zu https://github.com/CCDix/dobetr-de-cases
2. **Settings** → **Pages**
3. Source: `main` Branch, `/` Root
4. Save

→ Website erreichbar unter: `https://CCDix.github.io/dobetr-de-cases/`

---

### 4. **Custom Domain konfigurieren** (Optional)

Falls du `cases.dobetr.de` verwenden möchtest:
1. GitHub Settings → Pages → Custom domain: `cases.dobetr.de`
2. DNS-Provider: CNAME Record `cases` → `CCDix.github.io`

→ Website dann unter: `https://cases.dobetr.de`

---

## 🎨 Inhaltliche Verbesserungen (Optional)

- [ ] Echte Logos der drei Commissioner hinzufügen
- [ ] Case-spezifische Landingpages erstellen (`/dbl.html`, `/nuernberg.html`, `/ufl.html`)
- [ ] Testimonials von Coaches/Kommissären hinzufügen
- [ ] Assessment-Details & Ergebnisse dokumentieren
- [ ] Datenschutz & Impressum hinzufügen
- [ ] Analytics (Google Analytics oder Plausible) einbinden

---

## 📝 Struktur-Übersicht

```
dobetr-de-cases/
├── index.html              ← Hauptseite (3 Cases im Grid)
├── 404.html                ← Error Page
├── styles.css              ← dobetr.de Design (orange/blue/teal)
├── README.md               ← Dokumentation
├── DEPLOYMENT.md           ← Anleitung zum Hochladen
├── CNAME                   ← Custom Domain Konfiguration
├── _config.yml             ← GitHub Pages Config
├── .gitignore              ← Git Filter
└── assets/
    └── logos/
        └── README.md       ← Logo-Instruktionen
```

---

## 🚀 Go-Live Checkliste

- [ ] Alle Daten aktuell? (192 Athletes, 28, 67, etc.)
- [ ] Kontaktdaten korrekt? (hello@dobetr.de, +49-171-4863920)
- [ ] Links alle funktionsfähig?
- [ ] Logos hochgeladen?
- [ ] GitHub Repository erstellt?
- [ ] Pages aktiviert?
- [ ] Website testet? (Mobile & Desktop)

---

## 📞 Support

Bei Fragen oder Änderungen: **hello@dobetr.de**

