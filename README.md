# Continuous-Integration-Kurs

Das ist das Repository für die Übung im Kurs.

## Anleitung für einen Pull-Request

### 1.Fork
Zuerst wird das Repository mit Fork in den eigenen Bereich kopiert. Dazu muss der```Fork```-Button im Repository gedrückt werden.

### 2. Clone
Bevor ein Repository geklont werden kann, benötigt GitHub den eigenen SSH-Schlüssel. Dazu verwenden wird die Git GUI verwendet. Dort auf ```Help``` -> ```Show SSH Key``` klicken. Falls kein Key vorhanden ist, kann man einen neuen generieren lassen und optional ein Passwort setzen. Dieser Schlüssel muss in den GitHub Einstellungen auf ```SSH and GPG keys``` eingetragen werden. Danach kann Git lokal gestartet und das Repository mit den Befehlen geklont werden. Der Key kann in das Repository unter Code und SSH kopiert werden.
```bash
git clone [GitHub SSH Key]
```

### 3. New Branch 
Falls Änderungen vorgenommen werden müssen, empfiehlt es sich, diese in einem neuen Branch zu speichern. Dazu muss folgender Code in der Git-Bash eingegeben werden
```bash
git checkout -b [Branchname]
```
### 4. Commit
Wenn alle Änderungen vorgenommen wurden, commitet (speichert) man die Änderungen in sein Lokales Repository. Zuerst müssen alle Änderungen ausgewählt werden. Dazu wird dieser Code in der Git Bash benötigt.
```bash
git add .
``` 

Um die Änderungen zu speichern benötigt man diesen Code.
```bash
git commit -m"[Nachricht]"
```

### 5. Push
Um alle Änderungen auf GitHub hochzuladen, muss der Push-Befehl eingegeben werden. Dieser lautet
```bash
git push
```
Es kann sein, dass Git die Operation zunächst nicht zulässt, da der Branch kein Upstream ist. Git gibt jedoch den empfohlenen Code aus, um die Änderungen zu pushen. Dieser Code kann wie folgt aussehen
```bash
git push --set-upstream origin [Branchname]
```

### 6. Pull Request
Damit die Änderungen auch in dem Repository gespeichert werden, aus dem geforked wurde, wird ein Pull-Request benötigt. Der Pull-Request ist eine Anfrage an den Eigentümer des Repositories. Dieser kann entscheiden, ob die Änderungen übernommen werden sollen oder nicht. Wenn ihm etwas fehlt, kann er Kommentare hinzufügen. Einen Pull-Request erstellt man, indem man auf der Seite des Besitzers auf ```Pull-Request``` klickt. Dort klickt man auf ```New Pull Request```. Danach wählt man den Branch, in dem die Änderungen vorgenommen wurden und den Branch, in dem die Änderungen gespeichert werden sollen. Wenn alles ausgewählt ist, klickt man auf ```Create Pull Request```.

### 7. Sync Fork
Nachdem der Besitzer den Pul Request akzeptiert hat, muss der Stand wieder aktualisiert werden, damit die Änderungen auch im main-Branch vorhanden sind. Dazu gibt es einen Button ``Sync`` und dann auf ``Update Sync`` klicken.

### 8. Pull
Damit das Repository mit den Änderungen auch lokal gespeichert wird, muss man das Repository auf sein Profil ziehen. Dazu muss in der Git Bash folgender Code ausgeführt werden
```bash
git pull
```



