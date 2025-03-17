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
