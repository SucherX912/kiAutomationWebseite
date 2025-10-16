# Deployment-Anleitung für SmartFlow Automation Website

---

## 🚀 GitHub Pages Deployment (Empfohlen)

### Schritt 1: GitHub Repository erstellen

1. Gehe zu [GitHub](https://github.com) und melde dich an
2. Klicke auf **"New Repository"** (grüner Button oben rechts)
3. **Repository Name**: `smartflow-automation` (oder ein anderer Name)
4. **Description**: "KI-Automatisierung Website für SmartFlow Automation"
5. **Public** auswählen (für GitHub Pages kostenlos)
6. **NICHT** "Initialize with README" ankreuzen
7. Klicke auf **"Create repository"**

### Schritt 2: Code zu GitHub hochladen

Öffne ein Terminal/Command Prompt im `smartflow-website` Ordner und führe folgende Befehle aus:

```bash
# Repository-URL von GitHub kopieren (ersetze IHR-USERNAME und REPO-NAME)
git remote add origin https://github.com/IHR-USERNAME/smartflow-automation.git

# Code hochladen
git push -u origin main
```

**Beispiel:**
```bash
git remote add origin https://github.com/carstenmueller/smartflow-automation.git
git push -u origin main
```

### Schritt 3: GitHub Pages aktivieren

1. Gehe zu deinem Repository auf GitHub
2. Klicke auf **"Settings"** (Zahnrad-Icon)
3. Scrolle im linken Menü zu **"Pages"**
4. Unter **"Source"**:
   - Branch: **main**
   - Folder: **/ (root)**
5. Klicke auf **"Save"**
6. Warte 1-2 Minuten

### Schritt 4: Website aufrufen

Deine Website ist jetzt live unter:
```
https://IHR-USERNAME.github.io/smartflow-automation/
```

**Beispiel:**
```
https://carstenmueller.github.io/smartflow-automation/
```

---

## 🔧 Replit Deployment

### Option A: Repository importieren

1. Gehe zu [Replit](https://replit.com)
2. Klicke auf **"Create Repl"**
3. Wähle **"Import from GitHub"**
4. Gib deine Repository-URL ein
5. Klicke auf **"Import from GitHub"**
6. Klicke auf **"Run"**
7. Deine Website ist live!

### Option B: Dateien hochladen

1. Gehe zu [Replit](https://replit.com)
2. Klicke auf **"Create Repl"**
3. Wähle **"HTML, CSS, JS"** Template
4. Lösche alle vorhandenen Dateien
5. Lade alle Dateien aus dem `smartflow-website` Ordner hoch:
   - `index.html`
   - `styles.css`
   - `script.js`
   - Ordner `images/` mit allen Bildern
6. Klicke auf **"Run"**
7. Deine Website ist live!

### Replit öffentlich machen

1. Klicke auf den **"Share"** Button
2. Kopiere die **"Website URL"**
3. Teile diese URL mit deinen Kunden!

---

## 🌐 Netlify Deployment (Drag & Drop)

### Schritt 1: Netlify Account erstellen

1. Gehe zu [Netlify](https://www.netlify.com)
2. Klicke auf **"Sign up"** (kostenlos)
3. Melde dich mit GitHub, GitLab oder E-Mail an

### Schritt 2: Website hochladen

1. Gehe zu deinem Netlify Dashboard
2. Ziehe den gesamten `smartflow-website` Ordner auf die Seite (**Drag & Drop**)
3. Warte 10-30 Sekunden
4. Fertig! Deine Website ist live

### Schritt 3: Custom Domain (Optional)

1. Klicke auf **"Domain settings"**
2. Klicke auf **"Add custom domain"**
3. Gib deine Domain ein (z.B. `smartflow-automation.de`)
4. Folge den Anweisungen zur DNS-Konfiguration

---

## 🔗 Eigene Domain verbinden

### Für GitHub Pages:

1. Kaufe eine Domain (z.B. bei Namecheap, GoDaddy, Strato)
2. Gehe zu deinen Domain-DNS-Einstellungen
3. Füge folgende DNS-Records hinzu:

**A Records:**
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

**CNAME Record:**
```
www -> IHR-USERNAME.github.io
```

4. Gehe zu GitHub Repository → Settings → Pages
5. Unter **"Custom domain"** deine Domain eingeben
6. Warte 24-48 Stunden für DNS-Propagation

### Für Netlify:

1. Netlify Dashboard → Domain Settings
2. **"Add custom domain"**
3. Folge den Anweisungen (Netlify zeigt dir die DNS-Einstellungen)

---

## 📱 Testen vor dem Deployment

### Lokal testen:

1. **Option 1: Live Server (VS Code)**
   - Installiere "Live Server" Extension
   - Rechtsklick auf `index.html` → "Open with Live Server"

2. **Option 2: Python HTTP Server**
   ```bash
   cd smartflow-website
   python3 -m http.server 8000
   ```
   Öffne Browser: `http://localhost:8000`

3. **Option 3: Einfach Datei öffnen**
   - Doppelklick auf `index.html`
   - Öffnet sich im Standard-Browser

---

## ✅ Checkliste vor dem Go-Live

- [ ] Eigenes Foto in "Über mich"-Sektion eingefügt
- [ ] Preise überprüft und ggf. angepasst
- [ ] E-Mail-Adresse korrekt (`carsten.smartflow@gmail.com`)
- [ ] Alle Links funktionieren
- [ ] Mobile Ansicht getestet
- [ ] SEO-Meta-Tags überprüft
- [ ] Kontaktformular getestet
- [ ] Rechtschreibung geprüft

---

## 🐛 Troubleshooting

### Problem: Bilder werden nicht angezeigt

**Lösung:** Überprüfe, ob der `images/` Ordner korrekt hochgeladen wurde.

### Problem: CSS/JavaScript funktioniert nicht

**Lösung:** Überprüfe die Dateipfade in `index.html`:
```html
<link rel="stylesheet" href="styles.css">
<script src="script.js"></script>
```

### Problem: GitHub Pages zeigt 404

**Lösung:** 
- Warte 1-2 Minuten nach dem Aktivieren
- Überprüfe, ob `index.html` im Root-Verzeichnis liegt
- Stelle sicher, dass der Branch "main" ist

---

## 📧 Support

Bei Fragen oder Problemen:
- **E-Mail:** carsten.smartflow@gmail.com

---

## 🎉 Fertig!

Ihre Website ist jetzt live und bereit, Kunden zu gewinnen!

**Nächste Schritte:**
1. Website-URL in E-Mail-Signatur einfügen
2. Auf LinkedIn/Social Media teilen
3. Google My Business Profil erstellen
4. Google Analytics einrichten (optional)
5. Erste Kundengespräche führen!

Viel Erfolg mit SmartFlow Automation! 🚀

