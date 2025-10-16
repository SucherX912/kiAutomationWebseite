# Replit Setup-Anleitung für SmartFlow Automation

---

## 🎯 Was ist Replit?

Replit ist eine Online-Entwicklungsumgebung, mit der Sie Ihre Website direkt im Browser hosten und bearbeiten können – **ohne Installation, ohne Terminal, ohne Komplexität**.

**Vorteile:**
- ✅ Kostenlos für statische Websites
- ✅ Sofort live nach dem Upload
- ✅ Einfache Bearbeitung direkt im Browser
- ✅ Öffentliche URL zum Teilen
- ✅ Keine technischen Kenntnisse erforderlich

---

## 🚀 Schnellstart: Website auf Replit hochladen

### Schritt 1: Replit Account erstellen

1. Gehe zu [https://replit.com](https://replit.com)
2. Klicke auf **"Sign up"**
3. Melde dich an mit:
   - Google-Konto
   - GitHub-Konto
   - Oder E-Mail

### Schritt 2: Neues Repl erstellen

1. Klicke auf **"+ Create Repl"** (blauer Button)
2. Wähle **"HTML, CSS, JS"** als Template
3. **Title:** `SmartFlow Automation`
4. **Public** auswählen (damit die Website öffentlich ist)
5. Klicke auf **"Create Repl"**

### Schritt 3: Dateien hochladen

1. **Lösche** die vorhandenen Dateien (`index.html`, `style.css`, `script.js`)
2. Klicke auf die **drei Punkte** (⋮) neben "Files"
3. Wähle **"Upload file"** oder **"Upload folder"**
4. Lade folgende Dateien/Ordner hoch:
   - `index.html`
   - `styles.css`
   - `script.js`
   - `images/` (gesamter Ordner mit allen Bildern)
   - `README.md` (optional)

**Tipp:** Du kannst auch alle Dateien auf einmal per Drag & Drop hochladen!

### Schritt 4: Website starten

1. Klicke auf den grünen **"Run"** Button oben
2. Warte 5-10 Sekunden
3. Deine Website öffnet sich im rechten Fenster!

### Schritt 5: Öffentliche URL teilen

1. Klicke auf **"Share"** (oben rechts)
2. Kopiere die **"Website URL"** (z.B. `https://smartflow-automation.username.repl.co`)
3. Teile diese URL mit deinen Kunden!

---

## 🔧 Website auf Replit bearbeiten

### Text ändern:

1. Klicke auf `index.html` im Files-Panel
2. Finde den Text, den du ändern möchtest
3. Bearbeite den Text direkt
4. Klicke auf **"Run"** um die Änderungen zu sehen

### Farben ändern:

1. Klicke auf `styles.css`
2. Scrolle zu den CSS-Variablen (ganz oben):
   ```css
   :root {
       --primary-color: #0891b2;  /* Hier Farbe ändern */
       --secondary-color: #f97316;
   }
   ```
3. Ändere die Hex-Farbcodes
4. Klicke auf **"Run"**

### Eigenes Foto hinzufügen:

1. Lade dein Foto in den `images/` Ordner hoch (z.B. `carsten-mueller.jpg`)
2. Öffne `index.html`
3. Suche nach "Über mich"-Sektion (ca. Zeile 280)
4. Ersetze:
   ```html
   <div class="placeholder-image">
       <p>Ihr Foto hier</p>
   </div>
   ```
   mit:
   ```html
   <img src="images/carsten-mueller.jpg" alt="Carsten Müller" style="width: 100%; border-radius: 1rem;">
   ```
5. Klicke auf **"Run"**

---

## 🌐 Von GitHub zu Replit importieren

Falls Sie Ihre Website bereits auf GitHub haben:

### Schritt 1: Repository importieren

1. Klicke auf **"+ Create Repl"**
2. Wähle **"Import from GitHub"**
3. Gib deine Repository-URL ein:
   ```
   https://github.com/IHR-USERNAME/smartflow-automation
   ```
4. Klicke auf **"Import from GitHub"**

### Schritt 2: Starten

1. Klicke auf **"Run"**
2. Fertig! Deine Website ist live

### Schritt 3: Automatische Updates

Wenn du Änderungen auf GitHub machst:
1. Gehe zu Replit
2. Klicke auf **"Version Control"** (Git-Icon links)
3. Klicke auf **"Pull"**
4. Änderungen werden übernommen

---

## 💡 Replit Pro-Tipps

### Tipp 1: Custom Domain verbinden

Mit **Replit Hacker Plan** ($7/Monat) kannst du eine eigene Domain verbinden:
1. Gehe zu Repl Settings
2. Klicke auf **"Domains"**
3. Füge deine Domain hinzu (z.B. `smartflow-automation.de`)
4. Folge den DNS-Anweisungen

### Tipp 2: Always On

Standardmäßig schläft dein Repl nach Inaktivität. Mit **Always On** (Hacker Plan) bleibt es immer aktiv.

### Tipp 3: Versionskontrolle

Replit hat Git integriert:
- Klicke auf das **Git-Icon** (links)
- Committe Änderungen
- Pushe zu GitHub

### Tipp 4: Multiplayer-Bearbeitung

Lade andere ein, gemeinsam zu bearbeiten:
1. Klicke auf **"Share"**
2. Klicke auf **"Invite"**
3. Gib E-Mail-Adresse ein

---

## 📱 Mobile Bearbeitung

Replit funktioniert auch auf Tablets und Smartphones:
1. Öffne [replit.com](https://replit.com) im Browser
2. Melde dich an
3. Bearbeite deine Website unterwegs!

**Tipp:** Installiere die Replit Mobile App (iOS/Android) für bessere Erfahrung.

---

## 🔒 Sicherheit & Backups

### Automatische Backups:

Replit speichert automatisch alle Änderungen. Du kannst jederzeit zu früheren Versionen zurückkehren:
1. Klicke auf **"History"** (Uhr-Icon)
2. Wähle eine frühere Version
3. Klicke auf **"Restore"**

### Manuelles Backup:

1. Klicke auf die **drei Punkte** (⋮) neben "Files"
2. Wähle **"Download as zip"**
3. Speichere die ZIP-Datei auf deinem Computer

---

## ⚡ Performance-Optimierung

### Bilder komprimieren:

Große Bilder verlangsamen deine Website. Nutze Tools wie:
- [TinyPNG](https://tinypng.com)
- [Squoosh](https://squoosh.app)

### Caching aktivieren:

Füge eine `.htaccess` Datei hinzu (für Apache-Server):
```apache
<IfModule mod_expires.c>
  ExpiresActive On
  ExpiresByType image/png "access plus 1 year"
  ExpiresByType text/css "access plus 1 month"
  ExpiresByType application/javascript "access plus 1 month"
</IfModule>
```

---

## 🆘 Häufige Probleme & Lösungen

### Problem: "Run" Button macht nichts

**Lösung:**
- Warte 10 Sekunden
- Aktualisiere die Seite (F5)
- Überprüfe, ob `index.html` im Root liegt

### Problem: Bilder werden nicht angezeigt

**Lösung:**
- Überprüfe Dateipfade in `index.html`
- Stelle sicher, dass `images/` Ordner korrekt hochgeladen wurde
- Dateinamen sind case-sensitive: `Hero.png` ≠ `hero.png`

### Problem: CSS funktioniert nicht

**Lösung:**
- Überprüfe, ob `styles.css` im Root liegt
- Überprüfe den Link in `index.html`:
  ```html
  <link rel="stylesheet" href="styles.css">
  ```

### Problem: Website ist langsam

**Lösung:**
- Komprimiere Bilder
- Upgrade zu Replit Hacker Plan für bessere Performance
- Oder wechsle zu GitHub Pages (schneller)

---

## 🎓 Weiterführende Ressourcen

- **Replit Docs:** [https://docs.replit.com](https://docs.replit.com)
- **Replit Community:** [https://replit.com/talk](https://replit.com/talk)
- **HTML/CSS Tutorials:** [https://www.w3schools.com](https://www.w3schools.com)

---

## 📞 Support

Bei Fragen:
- **E-Mail:** carsten.smartflow@gmail.com
- **Replit Support:** [https://replit.com/support](https://replit.com/support)

---

## ✅ Checkliste: Replit Setup

- [ ] Replit Account erstellt
- [ ] Neues Repl erstellt
- [ ] Alle Dateien hochgeladen
- [ ] "Run" geklickt und Website getestet
- [ ] Öffentliche URL kopiert
- [ ] URL mit Kunden geteilt
- [ ] (Optional) Eigenes Foto hinzugefügt
- [ ] (Optional) Preise angepasst

---

## 🎉 Fertig!

Ihre Website ist jetzt live auf Replit!

**Nächste Schritte:**
1. URL in E-Mail-Signatur einfügen
2. Auf Social Media teilen
3. Erste Kunden gewinnen!

Viel Erfolg! 🚀

