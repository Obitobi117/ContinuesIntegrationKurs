# Git Begriffe

```bash
git status
```
Zeigt den derzeitigen Status an

```bash
git add  .
```
fügt alle derzeitigen Files hinzu (. steht als Platzhalter für alle veränderte Dateien)
```bash
git restore --staged <file>
```
Löscht die datei wieder aus dem Commit
```bash
git commit -m "comment"
```
Die Dateien aus git add . werden hier in die Repository geladen
```bash
git log
```
Zeigt alle udates und comments
```bash
git diff head^ head
```
"zeigt die Letzten Veränderungen an."
```bash
git init
```
erstellt eine Repository im derzeitigen Ordner
```bash
git remote set-url origin
```
Hiermit wird Lokal  die URL zum Upload verändert
```bash
git push -u origin Head:master
```
Local wird der brunch master und remote auch sonst kann man beides unterschiedlich nennen beim ersten Mal
```bash
git pull 
```
den aktuellen Branch Status ziehen
```bash
git clone 
```
Den Repository Klonen
```bash
git checkout -b 
```
Neuen Branch erstellen wichtig fürs pull request damit du nicht auf den master branch arbeites 
