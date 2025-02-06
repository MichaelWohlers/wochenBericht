Was genau machen wir hier?
- Wir machen eine Website für ein wochen bericht

Welche Funktionen haben wir hier?

- formular für den wochenbericht
- speichern der eingaben
- anzeigen der eingaben
- löschen der eingaben
- editieren der eingaben
- exportieren pdf, word, excel

Wer macht was?
- Elena: HTML css
- Konstantin: html css
- Michael: python, javascript
- Olha: sie macht ihre eigenes entwurf
- Mario: HTML

Wie ist die Projektstruktur?
- app/ (server logic)
- static/css/ (css)
- static/js/ (js)
- templates/ (html)

Wie ist die Git Branch Struktur?
- main (verteilbare Anwendung)
- staging (Testumgebung)
- feature/... (Features)
- bugfix/... (Bugfixes)



...

# Team Workflow Guide

Erste Einrichtung (einmalig)
   ```bash
   git clone https://github.com/MichaelWohlers/wochenBericht.git
   cd your-repo
   ```
Neue Funktion starten
   ```bash
   git checkout staging
   git pull origin staging
   git checkout -b feature/your-feature-name
   ```

3.Tägliche Arbeit
   ```bash
   # Get latest changes
   git checkout staging
   git pull origin staging
   git checkout your-feature-branch
   git merge staging

   # Work on code...

   # Commit changes
   git add .
   git commit -m "feat: what you did"
   git push origin your-feature-branch
   ```

