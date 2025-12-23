# 📋 Git-Anleitung für VS Code

## Schritt 1: Repository in VS Code öffnen

1. Öffne **Visual Studio Code**
2. Gehe zu **File** → **Open Folder**
3. Wähle deinen `Informatik_interaktiv` Ordner aus

## Schritt 2: Dateien hinzufügen

1. Kopiere die Dateien aus `repo_files/` in dein Repository:
   - `python/praesentation/index.html`
   - `python/praesentation/README.md`

2. In VS Code siehst du die neuen Dateien in der **Source Control** (Git Symbol in der Seitenleiste)

## Schritt 3: Änderungen committen

### Option A: VS Code GUI

1. Klicke auf das **Git Symbol** (links in der Seitenleiste)
2. Du siehst die neuen Dateien unter "Changes"
3. Klicke auf das **+** Symbol neben den Dateien (Stage Changes)
4. Schreibe eine Commit-Message oben, z.B.:
   ```
   Interaktive Python-Präsentation hinzugefügt
   
   - Live-Code-Ausführung im Browser
   - Syntax-Highlighting
   - 12 Folien mit Best Practice Tipps
   - Responsive Design für große Monitore
   ```
5. Klicke auf **✓ Commit**
6. Klicke auf **Sync Changes** (oder Push)

### Option B: Terminal in VS Code

1. Öffne das Terminal: **View** → **Terminal** (oder Ctrl+`)
2. Führe folgende Befehle aus:

```bash
# Dateien zur Staging Area hinzufügen
git add python/praesentation/index.html
git add python/praesentation/README.md

# Commit erstellen
git commit -m "Interaktive Python-Präsentation hinzugefügt

- Live-Code-Ausführung im Browser
- Syntax-Highlighting
- 12 Folien mit Best Practice Tipps
- Responsive Design für große Monitore"

# Zu GitHub pushen
git push origin main
```

(Falls dein Branch `master` heißt, nutze `git push origin master`)

## Schritt 4: Überprüfen

1. Gehe zu https://github.com/albecabrera/Informatik_interaktiv
2. Du solltest jetzt den Ordner `python/praesentation/` sehen
3. Die Präsentation ist online! 🎉

## 🆘 Bei Problemen

### "Git nicht gefunden"
- Installiere Git: https://git-scm.com/downloads

### "Authentication failed"
- Du musst dich bei GitHub anmelden
- In VS Code: Klicke auf das Account-Symbol unten links
- Wähle "Sign in with GitHub"

### "Branch nicht gefunden"
- Überprüfe deinen Branch-Namen: `git branch`
- Nutze den richtigen Namen beim Push

### "Merge Conflicts"
- Ziehe erst die neuesten Änderungen: `git pull`
- Löse Konflikte in VS Code
- Dann commit und push

## 📚 Nützliche Git-Befehle

```bash
# Status anzeigen
git status

# Alle Änderungen stagen
git add .

# Letzte Commits anzeigen
git log --oneline

# Änderungen von GitHub holen
git pull

# Branch wechseln
git checkout branch-name

# Neuen Branch erstellen
git checkout -b neuer-branch
```

---

**Tipp:** VS Code hat eine hervorragende Git-Integration! Die meisten Aktionen kannst du über die GUI machen.
