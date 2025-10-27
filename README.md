# 🎮 Neon Breakout - Arcade Game

Ein klassisches Breakout/Arkanoid Arcade-Spiel im modernen Neon-Design mit Highscore-System und Rangliste.

## 📋 Features

### Gameplay
- ✅ Klassisches Breakout-Gameplay mit Paddle, Ball und Blöcken
- 🖱️ Intuitive Maus-Steuerung für das Paddle
- 🎯 Realistische Ball-Physik mit dynamischen Abprallwinkeln
- 💥 6 Reihen mit 10 Blöcken pro Reihe (60 Blöcke pro Level)
- ⚡ Progressives Level-System mit steigender Schwierigkeit
- ❤️ 3 Leben pro Spiel
- 🏆 Punktesystem (obere Blöcke geben mehr Punkte)

### Highscore & Rangliste
- 📊 Echtzeit-Punkteanzeige während des Spiels
- 💾 Permanente Speicherung im Browser (localStorage)
- 🥇 Top 10 Rangliste mit Spielernamen und Punkten
- ✨ Automatische Highscore-Erkennung nach Game Over
- 🗑️ Möglichkeit zum Löschen der Rangliste

### Design
- 🌟 Modernes Neon-grün Design (#00ff00)
- 🌑 Dunkler Hintergrund für optimalen Kontrast
- ✨ Leuchteffekte (Glow) für alle Spielelemente
- 🎨 **Vollständig anpassbare Farben über CSS-Variablen**
- 📱 Responsive Design (funktioniert auf verschiedenen Bildschirmgrößen)
- 🎯 Custom Cursor (versteckt im Spielbereich)

### Technisch
- 📄 Standalone HTML-Datei (keine externen Abhängigkeiten)
- 🎨 HTML5 Canvas für optimale Performance
- 🔧 Vanilla JavaScript (keine Frameworks/Libraries erforderlich)
- 📦 Komplett einbettbar in Webflow und andere Plattformen
- 🚀 Sofort spielbar im Browser

---

## 🚀 Verwendung

### Lokal Spielen
1. Öffne die `index.html` Datei in einem modernen Browser (Chrome, Firefox, Safari, Edge)
2. Das Spiel startet automatisch mit dem Startbildschirm
3. Klicke auf "SPIEL STARTEN" und bewege die Maus, um zu spielen!

### Auf einem Webserver
1. Lade die `index.html` auf deinen Webserver hoch
2. Die Datei kann unter jedem beliebigen Namen gespeichert werden
3. Rufe die URL im Browser auf

---

## 🎨 Farbanpassung - So änderst du das Design

Die Farben des Spiels lassen sich sehr einfach anpassen! Alle Farben sind als **CSS-Variablen** im `<style>`-Bereich der HTML-Datei definiert.

### Wo findest du die Farbvariablen?
Öffne die `index.html` und suche nach diesem Abschnitt (ganz am Anfang des `<style>`-Tags):

```css
:root {
    /* Haupt-Neon-Farbe */
    --neon-primary: #00ff00;
    --neon-glow: rgba(0, 255, 0, 0.8);
    
    /* Hintergrundfarben */
    --bg-dark: #000000;
    --bg-overlay: rgba(0, 0, 0, 0.95);
    
    /* UI-Farben */
    --text-primary: #00ff00;
    --text-secondary: #00cc00;
    --border-color: #00ff00;
    
    /* Spiel-Element-Farben */
    --paddle-color: #00ff00;
    --ball-color: #00ff00;
    --block-color: #00ff00;
    --wall-color: #003300;
}
```

### Beispiele für Farbanpassungen

#### 🔴 Neon-Rot Design
```css
--neon-primary: #ff0000;
--neon-glow: rgba(255, 0, 0, 0.8);
--text-primary: #ff0000;
--text-secondary: #cc0000;
--border-color: #ff0000;
--paddle-color: #ff0000;
--ball-color: #ff0000;
--block-color: #ff0000;
--wall-color: #330000;
```

#### 🔵 Neon-Blau Design
```css
--neon-primary: #00ffff;
--neon-glow: rgba(0, 255, 255, 0.8);
--text-primary: #00ffff;
--text-secondary: #00cccc;
--border-color: #00ffff;
--paddle-color: #00ffff;
--ball-color: #00ffff;
--block-color: #00ffff;
--wall-color: #003333;
```

#### 💜 Neon-Lila Design
```css
--neon-primary: #ff00ff;
--neon-glow: rgba(255, 0, 255, 0.8);
--text-primary: #ff00ff;
--text-secondary: #cc00cc;
--border-color: #ff00ff;
--paddle-color: #ff00ff;
--ball-color: #ff00ff;
--block-color: #ff00ff;
--wall-color: #330033;
```

#### 🌈 Regenbogen/Mehrfarbig Design
```css
--neon-primary: #00ff00;
--neon-glow: rgba(0, 255, 0, 0.8);
--text-primary: #00ffff;      /* Cyan für Text */
--border-color: #ff00ff;      /* Magenta für Rahmen */
--paddle-color: #ffff00;      /* Gelb für Paddle */
--ball-color: #ff0000;        /* Rot für Ball */
--block-color: #00ff00;       /* Grün für Blöcke */
--wall-color: #0000ff;        /* Blau für Wände */
```

### 💡 Tipps zur Farbanpassung

1. **Hex-Farbcodes verwenden**: `#RRGGBB` Format (z.B. `#ff0000` für Rot)
2. **RGB/RGBA für Transparenz**: `rgba(R, G, B, Alpha)` - Alpha ist 0-1 für Transparenz
3. **Dunklen Hintergrund beibehalten**: `--bg-dark: #000000;` für beste Sichtbarkeit
4. **Glow-Farbe anpassen**: Die `--neon-glow` sollte zur Hauptfarbe passen (gleiche RGB-Werte, nur mit Alpha-Kanal)
5. **Kontrast beachten**: Helle Neon-Farben auf dunklem Hintergrund funktionieren am besten

---

## 🌐 Einbettung in Webflow

### Option 1: Embed-Code-Block (Empfohlen)

1. **In Webflow:**
   - Füge ein **Embed**-Element zu deiner Seite hinzu
   - Wähle "Custom Code" aus

2. **Kopiere diesen Code in den Embed-Block:**

```html
<iframe 
    src="https://DEINE-DOMAIN.com/pfad/zu/index.html" 
    width="100%" 
    height="900px" 
    frameborder="0" 
    style="border: none; max-width: 900px; margin: 0 auto; display: block;">
</iframe>
```

3. **Ersetze `https://DEINE-DOMAIN.com/pfad/zu/index.html`** mit der URL zu deiner hochgeladenen `index.html` Datei

4. **Passe die Höhe an** (`height="900px"`), falls nötig

### Option 2: Direkteinbettung (Für fortgeschrittene Benutzer)

Wenn du den Code direkt in Webflow einbetten möchtest:

1. Füge ein **HTML Embed**-Element hinzu
2. Kopiere den **gesamten Inhalt** der `index.html` Datei
3. Füge ihn in den Embed-Block ein

**⚠️ Hinweis:** Diese Methode kann bei sehr großem Code zu Performance-Problemen führen. Die iframe-Methode (Option 1) ist empfehlenswerter.

### Option 3: GitHub Pages + Webflow

1. **Upload zu GitHub:**
   - Erstelle ein neues Repository auf GitHub
   - Lade die `index.html` hoch
   - Aktiviere GitHub Pages in den Repository-Einstellungen

2. **In Webflow einbetten:**
   - Verwende die GitHub Pages URL in einem iframe (siehe Option 1)
   - Beispiel: `https://dein-username.github.io/breakout-game/index.html`

---

## 📁 Dateistruktur

```
breakout-game/
│
├── index.html          # Das komplette Spiel (HTML + CSS + JavaScript)
└── README.md          # Diese Dokumentation
```

---

## 🎮 Spielanleitung

### Steuerung
- **Maus**: Bewege die Maus horizontal, um das Paddle zu steuern
- Das Paddle folgt automatisch der Maus-Position

### Spielziel
- Zerstöre alle Blöcke mit dem Ball
- Verhindere, dass der Ball unten rausfällt
- Erreiche einen möglichst hohen Score

### Punktesystem
- **Oberste Reihe**: 60 Punkte pro Block
- **2. Reihe**: 50 Punkte pro Block
- **3. Reihe**: 40 Punkte pro Block
- **4. Reihe**: 30 Punkte pro Block
- **5. Reihe**: 20 Punkte pro Block
- **Unterste Reihe**: 10 Punkte pro Block

### Schwierigkeit
- Mit jedem Level steigt die Ball-Geschwindigkeit
- Die Herausforderung wird kontinuierlich größer
- Strategie: Ziele zuerst auf die oberen, wertvolleren Blöcke!

---

## 🔧 Technische Details

### Browser-Kompatibilität
- ✅ Chrome/Edge (empfohlen)
- ✅ Firefox
- ✅ Safari
- ✅ Opera
- ✅ Alle modernen Browser mit HTML5-Unterstützung

### Voraussetzungen
- JavaScript muss aktiviert sein
- localStorage muss verfügbar sein (für Highscore-Speicherung)
- HTML5 Canvas Unterstützung

### Datenspeicherung
- **LocalStorage Key**: `breakoutLeaderboard`
- **Datenformat**: JSON Array mit Top 10 Scores
- **Speicherort**: Browser des Benutzers (keine Server-Kommunikation)
- **Datenschutz**: Alle Daten bleiben lokal, keine Übertragung an externe Server

---

## 🛠️ Anpassungen & Erweiterungen

### Schwierigkeitsgrad anpassen

**Ball-Geschwindigkeit ändern:**
```javascript
// Suche in der HTML nach:
const ball = {
    radius: 8,
    x: canvas.width / 2,
    y: canvas.height / 2,
    dx: 4,        // ← Horizontale Geschwindigkeit
    dy: -4,       // ← Vertikale Geschwindigkeit
    speed: 4      // ← Basis-Geschwindigkeit
};
```

**Paddle-Größe ändern:**
```javascript
const paddle = {
    width: 120,   // ← Breite des Paddles (Standard: 120)
    height: 15,   // ← Höhe des Paddles
    // ...
};
```

**Anzahl der Leben ändern:**
```javascript
let lives = 3;   // ← Anzahl der Leben (Standard: 3)
```

### Block-Layout ändern

```javascript
const blockConfig = {
    rows: 6,       // ← Anzahl der Reihen (Standard: 6)
    cols: 10,      // ← Anzahl der Spalten (Standard: 10)
    width: 70,     // ← Breite eines Blocks
    height: 25,    // ← Höhe eines Blocks
    padding: 10,   // ← Abstand zwischen Blöcken
    // ...
};
```

### Canvas-Größe anpassen

```html
<!-- Im HTML suchen: -->
<canvas id="gameCanvas" width="800" height="600"></canvas>

<!-- Ändere width und height nach Bedarf -->
```

---

## 📝 Lizenz & Credits

Dieses Spiel wurde als Open-Source-Projekt entwickelt und kann frei verwendet, modifiziert und verteilt werden.

### Verwendung
- ✅ Privat verwenden
- ✅ Kommerziell verwenden
- ✅ Modifizieren und anpassen
- ✅ In eigene Projekte einbetten
- ✅ Auf Webseiten hosten

### Credits
Entwickelt mit ❤️ und modernem Web-Technologie-Stack:
- HTML5 Canvas
- Vanilla JavaScript (ES6+)
- CSS3 mit Animations & Effekten

---

## 🐛 Bekannte Probleme & Lösungen

### Problem: Spiel lädt nicht
**Lösung**: Stelle sicher, dass JavaScript im Browser aktiviert ist

### Problem: Highscores werden nicht gespeichert
**Lösung**: 
- Prüfe ob localStorage im Browser aktiviert ist
- Im Inkognito-Modus funktioniert localStorage möglicherweise nicht
- Prüfe Browser-Einstellungen für Cookies/Speicher

### Problem: Canvas ist zu groß/klein
**Lösung**: Passe die Canvas-Größe im HTML an (siehe "Canvas-Größe anpassen")

### Problem: Spiel ist zu schwer/leicht
**Lösung**: Passe Geschwindigkeit, Paddle-Größe oder Anzahl der Leben an (siehe "Schwierigkeitsgrad anpassen")

---

## 📞 Support & Feedback

Für Fragen, Anregungen oder Bug-Reports:
- Öffne ein Issue auf GitHub
- Kontaktiere den Entwickler
- Erstelle einen Pull Request für Verbesserungen

---

## 🎯 Roadmap & Mögliche Erweiterungen

Ideen für zukünftige Features:
- [ ] Power-Ups (Multi-Ball, größeres Paddle, etc.)
- [ ] Sound-Effekte und Hintergrundmusik
- [ ] Verschiedene Block-Typen (mehrfache Treffer, unzerstörbar, etc.)
- [ ] Mobile Touch-Steuerung
- [ ] Online-Leaderboard mit Backend
- [ ] Achievements/Errungenschaften
- [ ] Verschiedene Themes/Skins
- [ ] Partikel-Effekte bei Block-Zerstörung
- [ ] Boss-Level
- [ ] Multiplayer-Modus

---

## 🌟 Viel Spaß beim Spielen!

**Tipp**: Versuche alle Level zu schaffen und deinen Highscore zu knacken! 🏆

---

**Version**: 1.0.0  
**Letzte Aktualisierung**: Oktober 2025  
**Sprache**: Deutsch (DE)
