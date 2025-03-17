# Git

[Wikipedia-Artikel](https://de.wikipedia.org/wiki/Git)

## Webseiten, die Git nutzen

- [GitHub](https://github.com/)
- [GitLab](https://about.gitlab.com/)
- [BitBucket](https://bitbucket.org/)

## Vorbereiten der Benutzung von Git mit GitHub

- Anlegen eines Accounts. Verwende für den Namen deines Accounts Kleinbuchstaben (im Beispiel `monalisa`)!
- Einrichten von 2FA
- Lokale Installation von Git auf deinem Rechner
- Setze globale Einstellungen für Git auf deinem Rechner. Verwende nicht deine echte E-Mailadresse:

  ```git config --global user.name "Mona Lisa"```

  ```git config --global user.email monalisa@users.noreply.github.com```

  ```git config --global init.defaultBranch main```

  Optional kannst du einrichten, dass du das später zu erzeugende Token auf deinem Rechner speichern möchtest:

  ```git config --global credential.helper store```
  
- Es gibt zwei Protokolle, um mit GitHub zu kommunizieren: HTTPS und SSH
  SSH funktioniert aus der Hochtaunusschule nicht, weil du nicht durch die Firewall kommst.

- Um mit HTTPS auf deinem Repo Updates zu machen, benötigst du ein Personal Access Token (PAT).
  Das kannst du so erzeugen:
  - Klicke in GitHub auf das Symbol rechts oben, welches für deinen Account steht!
  - Gehe auf Settings!
  - Gehe dann links ganz unten auf Developer Settings!
  - Gehe auf Personal Access Tokens
  - Generiere ein neues (classic) Token!
  - Setze die Expiration auf "No expiration"
  - Bei "Scopes" wähle alle von "Repo" aus!
  - Klicke dann ganz unten auf "Generate Token"!
  - Das generierte Token wird dir angezeigt. Sichere es dir. Es kann später nicht noch einmal angezeigt werden. Du kannst jedoch jederzeit das Token löschen und ein neues Generieren.
 
## Anlegen eines Repositories auf GitHub

Du kannst dann auf GitHub ein neues Projekt anlegen. Für den Namen werden Kleinbuchstaben empfohlen. Akzeptiere den Vorschlag, dass eine neue Datei mit dem Namen `README.md` angelegt wird. Diese Datei dient der Dokumentation und wird automatisch für dein Projekt angezeigt.

## Klonen deines neuen Projektes auf deinen Rechner

Wenn du das Projekt mit der Datei `README.md` angelegt hast, dann kannst du auf den grünen Button klicken und dir die URL für HTTPS kopieren.

Erzeuge dir auf deinem Rechner einen Ordner für alle zukünftigen Ordner, z.B. `/home/monalisa/src`!

Führe dann in diesem Ordner ein `git clone` aus mit der gerade eben kopierten HTTPS-URL, z.B.

```git clone https://github.com/monalisa/project1.git```

Du bekommst dann einen Ordner namens `project1` im Beispiel, der dann deine `README.md` enthält. Du kannst diesen Ordner mit deiner IDE öffnen, z.B. VS Code und kannst Änderungen an deinem Projekt vornehmen.

## Änderungen an GitHub übertragen

Alle Dateien, deren Änderungen gespeichert werden sollen, müssen zu einer sog. Staging Area zugefügt werden. Du kannst z.B. das Kommando

```git add .```

ausführen. Damit werden alle Dateien zur Staging Area zugefügt.

Alle vorgemerkten Dateien werden mit dem nächsten Kommando in die Versionshistorie eingetragen. Die Änderung ist damit durchgeführt:

```git commit -m "Update README.md"```

Aus der Message sollte hervorgehen, was du gemacht hast.

Bis jetzt wurden deine Änderungen nur lokal auf deinem Rechner ausgeführt. Das funktioniert also alles auch ohne Netz. Wenn du die lokalen Änderungen an GitHub übertragen möchtest, verwende das Kommando

```git push```

Die Änderungen sind dann auch auf der Webseite von GitHub zu sehen. Wenn du auf der Webseite Änderungen an deinen Dateien durchführst, kannst du diese Änderungen auf deinen Rechner herunterladen mit dem Kommando

```git pull```

## Auf GitHub oder lokal starten? Wichtige Hinweise

Entweder du beginnst mit einem neuen Projekt auf GitHub, fügst eine `README.md` hinzu und klonst dann das Projekt auf deinen Rechner.

Wenn du jedoch lokal beginnen möchtest, und noch kein Projekt auf GitHub hast, dann kannst du dein leeres Repository auch lokal erzeugen mit dem Kommando

```git init```

Du kannst dann deine Änderungen alle lokal auf deinen Rechner "committen". Falls du dann später doch ein Repository auf GitHub anlegen möchtest, achte darauf, diesmal *keine* `README.md` oder eine andere Datei zuzufügen! GitHub zeigt dir an, wie du dein lokales Repository auf GitHub hochladen kannst.

## Mit anderen Leuten zusammenarbeiten

Wenn du ganz alleine an einem Projekt arbeitest, wirst du keinen anderen stören. Möchtest du aber mit anderen Leuten zusammarbeiten an einem Projekt, besteht die Gefahr, dass ihr euch möglicherweise gegenseitig behindert.

Dazu kennt Git das Konzept der Verzweigungen - Branches. Wenn du alleine arbeitest, dann benutzt du vielleicht nur den Branch mit dem Namen `main`. In der Vergangenheit nannte man diesen Branch `master`. 

Wenn du mit anderen Leuten zusammenarbeitest, werden die anderen Leute sicherlich andere Teile des Projekts bearbeiten. Damit jede(r) Mitarbeiter/in für sich ungestört arbeiten kann, erzeugt er/sie sich einen Branch für die aktuelle Aufgabe, die gerade von ihm/ihr bearbeitet wird.

Diesen Branch kannst du zuerst lokal erzeugen auf deinem PC. Deine Änderungen machst du dann ausschließlich auf deisem Branch. Bist du fertig mit deinen Änderungen, dann veröffentlichst du deinen Branch auf GitHub. Noch ist der `main`-Branch davon nicht beeinflusst.

Möchtest du noch Änderungen in deinem Branch durchführen, kannst du das jederzeit tun und die Änderungen wieder zu GitHub schicken.

Wenn du zu der Überzeugung gelangt bist, dass dein Branch nun in den `main`-Branch integriert werden soll, dann erstellst du dafür einen Pull-Request.

Jemand, der dazu berechtigt ist, vielleicht auch du selbst, schaut sich deinen Pull-Request an und prüft, ob dein Branch nun in den `main`-Branch integriert werden kann und soll. Wird der Pull-Request bestätigt, sind deine Änderungen dann ab sofort im `main`-Branch integriert.

Wechsle auf deinem Computer wieder auf den `main`-Branch zurück und führe ein `git pull` durch! Damit holst du dir den aktuellen Stand des `main`-Branches von GitHub, der nun auch deine Änderungen enthält. Der Branch, den du vorher auf deinem Gerät erstellt hast, wird jetzt nicht mehr benötigt und du solltest ihn nun löschen.

Möchtest du eine weitere Änderung erstellen, erzeuge dir wieder einen neuen Branch aus dem aktuellen `main`-Branch.
