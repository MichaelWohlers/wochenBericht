Start App:
1. pip install flask
2. cd app
3. flask run
4. open http://127.0.0.1:5000/



Was genau machen wir hier?
- Wir machen eine Website für ein wochen bericht

Welche Funktionen haben wir hier?


Wer macht was?


Wie ist die Projektstruktur?


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

