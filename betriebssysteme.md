# Betriebssysteme

Grundlage: [Kerncurriculum Fachoberschule](https://kultus.hessen.de/sites/kultus.hessen.de/files/2023-08/kc_fos_informationstechnik_2022.pdf) Kapitel 12.8 Administration eines Betriebssystems Seite 51

HINWEIS: Wir betrachten hier ausschließlich UNIX/Linux

## Allgemeines

### Geschichte von Betriebssystemen
### Aufbau, Architektur
### Distributionen

Wichtige Distributionen bei Linux sind Debian/Ubuntu und Fedora/RedHat-Enterprise-Linux (RHEL) OpenSuSE/SLES

## Dateiverwaltung

### Namenskonventionen, Dateitypen

Namenskonventionen: Kaum Einschränkungen
Dateitypen: Textdateien, Binärdateien, Ausführbare Dateien

### Absolute und relative Dateinamen

Absoluter Pfad geht mit "/" los, relativer Pfad nicht.

Aufgaben:

- Du befindest dich im Ordner `/Users/schule`. Das Kommando `ls` zeigt den Ordner `foo` an. Gib den absoluten
  Pfad des Ordners `foo` an!
- Du befindest dich im Ordner `/Users/schule/foo`. Gib den relativen Pfad zur Datei `/Users/schule/bar/baz.txt` an!

### Verzeichnisbaum und Dateisysteme

Die Wurzel des Baums wird mit "/" bezeichnet.
Kommandos df und du

### Umgang mit Dateien (Kopieren, Erstellen, Verschieben, Löschen, Inhalte anzeigen, Archivieren, Komprimieren)

- `cp`
- `touch`
- `mv` 
- `rm`
- `rmdir`
- `cat`
- `more`

Aufgaben:

- Erkläre die Wirkung der oben genanten Kommandos!
- Wann kann das Kommando `rmdir` nicht verwendet werden?
- Welches Kommondo muss ich benutzen und welche Aufrufoption muss ich mitgeben, um einen Ordner mit Inhalt zu löschen?
- Welche Aufrufoption muss ich bei `rm` mitgeben, um schreibgeschützte Dateien zu löschen?

### Suchmuster für Dateien, reguläre Ausdrücke
### Ein- und Ausgabeumlenkung und Kommandopipelines
### Texteditor
