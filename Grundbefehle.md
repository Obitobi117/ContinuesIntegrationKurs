Git Begriffe:

git status 
Zeigt den derzeitigen Status an

git add  . 
fügt alle derzeitigen Files hinzu (. steht als Platzhalter für alle veränderte Dateien)

git restore --staged <file> 
Löscht die datei wieder aus dem Commit

git commit -m "comment"
Die Dateien aus git add . werden hier in die Repository geladen

git log 
Zeigt alle udates und comments

git diff head^ head 
zeigt die Letzten Veränderungen an.

git init 
erstellt eine Repository im derzeitigen Ordner

git remote set-url origin
Hiermit wird Lokal  die URL zum Upload verändert

git push -u origin Head:master
Local wird der brunch master und remote auch sonst kann man beides unterschiedlich nennen beim ersten Mal

git pull 
den aktuellen Branch Status ziehen

git clone 
Den Repository Klonen

git checkout -b 
Neuen Branch erstellen wichtig fürs pull request damit du nicht auf den master branch arbeites 
