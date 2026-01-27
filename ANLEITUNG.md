# ❤️ Valentinstag-Website - Anleitung für Anfänger

## 📋 Schnellstart-Checkliste

### ✅ Schritt 1: Dateien vorbereiten
- [ ] Alle 3 Dateien in einem Ordner speichern:
  - `index.html`
  - `style.css`
  - `script.js`

### ✅ Schritt 2: Bilder hochladen
- [ ] Erstelle einen Unterordner namens `img` im selben Verzeichnis
- [ ] Lade folgende Bilder in den `img` Ordner hoch:
  - `hero.jpg` - Hauptbild im Hero-Bereich (idealerweise 800x600px)
  - `1.jpg` - Galerie Bild 1 (idealerweise 800x500px)
  - `2.jpg` - Galerie Bild 2
  - `3.jpg` - Galerie Bild 3
  - `4.jpg` - Galerie Bild 4

**Tipp:** Bilder sollten im JPG oder PNG Format sein und nicht zu groß (max. 2MB pro Bild).

---

## 🎨 Personalisierung

### 1️⃣ PASSWORT ÄNDERN
**Wo:** `script.js` (Zeile 7)

```javascript
const PASSWORD = "liebe"; // ← Hier dein Wunschwort eintragen
```

**Beispiel:**
```javascript
const PASSWORD = "valentinstag2025";
```

---

### 2️⃣ GRÜNDE BEARBEITEN
**Wo:** `script.js` (Zeile 10-22)

```javascript
const REASONS = [
    "Weil dein Lächeln mein Herz jedes Mal zum Schmelzen bringt.",
    "Weil du mich verstehst, auch wenn ich nichts sage.",
    // ... füge deine eigenen Gründe hinzu
];
```

**Tipps:**
- Mindestens 6 Gründe, maximal beliebig viele
- Jeder Grund in Anführungszeichen
- Mit Komma am Ende (außer beim letzten)

---

### 3️⃣ BILDUNTERSCHRIFTEN ÄNDERN
**Wo:** `index.html` (suche nach `<figcaption class="slide-caption">`)

Finde diese Zeilen und ändere die Texte:

```html
<figcaption class="slide-caption">Unser erster gemeinsamer Tag</figcaption>
<figcaption class="slide-caption">Lachen und Abenteuer</figcaption>
<figcaption class="slide-caption">Gemeinsame Träume</figcaption>
<figcaption class="slide-caption">Für immer und einen Tag</figcaption>
```

---

### 4️⃣ LIEBESBRIEF ANPASSEN
**Wo:** `index.html` (suche nach `<div class="letter-paper">`)

Ersetze den gesamten Text zwischen `<p class="letter-text">` und `</p>`:

```html
<p class="letter-text">
    Mein Liebling,<br><br>
    
    [DEIN BRIEFTEXT HIER]<br><br>
    
    <span class="letter-signature">— Dein Name ❤️</span>
</p>
```

**Wichtig:** Nutze `<br><br>` für Absätze!

---

### 5️⃣ GEHEIME NACHRICHT ÄNDERN
**Wo:** `index.html` (suche nach `<div class="secret-reveal">`)

```html
<div class="secret-reveal hidden" id="secretReveal">
    <div class="unlock-icon">🔓</div>
    <h3>Überraschung! 🎉</h3>
    <p>
        [DEINE GEHEIME NACHRICHT HIER]
        Zum Beispiel: Eine Überraschungsreise, ein Date, etc.
    </p>
</div>
```

---

### 6️⃣ MUSIK HINZUFÜGEN (Optional)

#### Option A: Spotify
**Wo:** `index.html` (suche nach `SPOTIFY_SONG_ID`)

1. Gehe zu deinem Lieblingssong auf Spotify
2. Klicke auf die 3 Punkte → Teilen → Song-Link kopieren
3. Beispiel-Link: `https://open.spotify.com/track/3n3Ppam7vgaVa1iaRUc9Lp`
4. Die Song-ID ist der Teil nach `/track/`: `3n3Ppam7vgaVa1iaRUc9Lp`
5. Ersetze in der HTML:

```html
<iframe 
    src="https://open.spotify.com/embed/track/3n3Ppam7vgaVa1iaRUc9Lp?utm_source=generator&theme=0"
    ...
</iframe>
```

#### Option B: YouTube
1. Lösche den gesamten Spotify-`<iframe>` Block
2. Entferne die `<!-- -->` Kommentare beim YouTube-Block
3. Finde dein YouTube-Video und kopiere die Video-ID aus der URL
4. Beispiel: `https://www.youtube.com/watch?v=dQw4w9WgXcQ` → ID = `dQw4w9WgXcQ`
5. Ersetze `YOUTUBE_VIDEO_ID`:

```html
<iframe 
    src="https://www.youtube.com/embed/dQw4w9WgXcQ?autoplay=1"
    ...
</iframe>
```

---

## 🚀 GitHub Pages Deployment

### Schritt-für-Schritt:

1. **GitHub Account erstellen** (falls noch nicht vorhanden)
   - Gehe zu [github.com](https://github.com)
   - Klicke "Sign up"

2. **Neues Repository erstellen**
   - Klicke oben rechts auf das "+" Symbol
   - Wähle "New repository"
   - Repository Name: z.B. `valentinstag-website`
   - Wähle "Public"
   - Klicke "Create repository"

3. **Dateien hochladen**
   - Klicke "uploading an existing file"
   - Ziehe alle Dateien rein:
     - `index.html`
     - `style.css`
     - `script.js`
     - Den kompletten `img` Ordner mit allen Bildern
   - Klicke "Commit changes"

4. **GitHub Pages aktivieren**
   - Gehe zu "Settings" (oben im Repository)
   - Scrolle zu "Pages" (linkes Menü)
   - Bei "Source": Wähle "Deploy from a branch"
   - Bei "Branch": Wähle "main" und "/ (root)"
   - Klicke "Save"

5. **Warte 1-2 Minuten**
   - GitHub baut deine Seite
   - Refresh die Seite
   - Du siehst oben einen grünen Kasten mit deiner URL

6. **Deine Website ist live! 🎉**
   - URL: `https://dein-username.github.io/valentinstag-website`

---

## 🎨 Farbschema wechseln

Die Website hat 3 verschiedene Farbschemata:

1. **Default** (Hell Valentinstag) - Weiß/Rot/Pink
2. **Rose** (Pinker) - Intensivere Rosatöne
3. **Night** (Dunkel Romantisch) - Dunkler Hintergrund mit rosafarbenen Akzenten

**Wechseln:** Klicke auf den 🎨 Button oben rechts!

---

## 🎬 Cinematic Trailer

Die Website startet mit einer **Trailer-Animation**:

1. **Türen öffnen sich** (2 Sekunden)
2. **Laptop erscheint** mit pulsierendem Herz (2 Sekunden)
3. **Zoom-Effekt** in den Bildschirm (2 Sekunden)
4. **Website lädt** (smooth transition)

**Überspringen:** Klicke unten rechts auf "Überspringen →"

---

## 🔧 Häufige Probleme & Lösungen

### ❌ Bilder werden nicht angezeigt
**Lösung:**
- Prüfe, ob der `img` Ordner korrekt hochgeladen wurde
- Prüfe die Dateinamen (müssen exakt `hero.jpg`, `1.jpg`, etc. heißen)
- Achte auf Groß-/Kleinschreibung!

### ❌ Musik spielt nicht ab
**Lösung:**
- Stelle sicher, dass die Song-ID/Video-ID korrekt ist
- Bei Spotify: Prüfe, ob der Song öffentlich verfügbar ist
- Klicke zuerst auf den "Abspielen" Button (Autoplay ist blockiert)

### ❌ Passwort funktioniert nicht
**Lösung:**
- Prüfe in `script.js` Zeile 7: `const PASSWORD = "..."`
- Groß-/Kleinschreibung wird ignoriert
- Keine Leerzeichen vor/nach dem Passwort

### ❌ GitHub Pages zeigt 404 Fehler
**Lösung:**
- Warte 2-5 Minuten nach dem ersten Deployment
- Prüfe, ob die `index.html` im Root-Verzeichnis liegt (nicht in einem Unterordner)
- Prüfe Settings → Pages → Branch muss auf "main" stehen

---

## 💡 Weitere Anpassungen

### Beziehungsdatum ändern
**Wo:** `script.js` (Zeile 25)

```javascript
const RELATIONSHIP_START = new Date('2022-12-29T00:00:00');
```

Ändere das Datum im Format `YYYY-MM-DDTHH:MM:SS`

### Name/Spitzname ändern
Suche in `index.html` nach:
- "mein Herz" → Dein Spitzname
- "Dein Reni" → Dein Name

---

## 📱 Mobile Optimierung

Die Website ist **vollständig responsive**:
- ✅ Touch-Swipe im Carousel
- ✅ Optimierte Schriftgrößen
- ✅ Angepasste Button-Größen
- ✅ Mobile-friendly Trailer

Teste die Website auf deinem Handy!

---

## ❤️ Viel Erfolg!

Bei Fragen oder Problemen:
- Prüfe die Konsole im Browser (F12 → Console)
- Kontrolliere, ob alle Dateien korrekt hochgeladen wurden
- Stelle sicher, dass keine Sonderzeichen in Dateinamen sind

**Frohen Valentinstag! 🌹**
