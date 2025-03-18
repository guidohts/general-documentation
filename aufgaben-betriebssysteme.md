# Aufgaben Betriebssysteme

## Dateisysstemkommandos

Dateioperationen
cp (Kopieren)

    Erstelle eine Datei namens "original.txt" und kopiere sie zu "kopie.txt".

    Kopiere den Inhalt eines Verzeichnisses in ein neues Verzeichnis.

touch (Dateien erstellen/Zeitstempel aktualisieren)

    Erstelle drei leere Dateien namens "datei1.txt", "datei2.txt" und "datei3.txt".

    Aktualisiere den Zeitstempel einer existierenden Datei, ohne ihren Inhalt zu ändern.

mv (Verschieben/Umbenennen)

    Benenne "datei1.txt" in "neu1.txt" um.

    Verschiebe "datei2.txt" in ein Unterverzeichnis.

rm (Löschen von Dateien)

    Lösche die Datei "datei3.txt".

    Lösche mehrere Dateien auf einmal mit einem Befehl.

rmdir (Löschen von leeren Verzeichnissen)

    Erstelle ein leeres Verzeichnis und lösche es wieder.

    Versuche, ein nicht-leeres Verzeichnis zu löschen und beobachte das Ergebnis.

Textanzeige
cat (Anzeigen von Dateiinhalten)

    Zeige den Inhalt von "neu1.txt" an.

    Verbinde den Inhalt von zwei Dateien und zeige das Ergebnis an.

more (Seitenweise Anzeige)

    Zeige den Inhalt einer langen Textdatei seitenweise an.

    Suche nach einem bestimmten Wort in der angezeigten Datei.

Kombinierte Aufgabe

Erstelle ein Skript, das folgende Schritte ausführt:

    Erstellt ein Verzeichnis "uebung".

    Wechselt in dieses Verzeichnis.

    Erstellt drei Dateien mit touch.

    Kopiert eine der Dateien.

    Benennt eine Datei um.

    Fügt Text in eine Datei ein und zeigt ihn an.

    Löscht eine Datei und das Verzeichnis.

### Suchmuster für Dateien - Reguläre Ausdrücke

Aufgaben mit dem Platzhalter ?

    Erstelle drei Dateien namens "datei1.txt", "datei2.txt" und "datei3.txt". Verwende dann den Befehl ls datei?.txt, um alle diese Dateien aufzulisten.

    Erstelle Dateien mit den Namen "a1.log", "b2.log" und "c3.log". Benutze den Befehl mv ??.log logs/, um alle diese Dateien in ein Verzeichnis namens "logs" zu verschieben.

    Kopiere alle Dateien, die genau fünf Zeichen im Namen haben und mit ".txt" enden, in ein Backup-Verzeichnis: cp ?????.txt backup/

Aufgaben mit dem Platzhalter *

    Liste alle Dateien in deinem aktuellen Verzeichnis auf, die mit "test" beginnen: ls test*

    Lösche alle Dateien mit der Endung ".tmp" im aktuellen Verzeichnis: rm *.tmp

    Verschiebe alle JPEG-Bilder (Endungen .jpg oder .jpeg) in einen Ordner namens "Bilder": mv *.jp* Bilder/

Kombinierte Aufgaben

    Erstelle ein Skript, das alle Textdateien (.txt) findet, deren Namen mit einem Buchstaben beginnen und eine einstellige Zahl enthalten: ls [a-z]*[0-9]*.txt

    Schreibe ein Kommando, das alle Dateien anzeigt, die genau drei Zeichen vor dem Punkt in ihrem Namen haben, unabhängig von der Dateiendung: ls ???.*

    Erstelle ein Backup aller Konfigurationsdateien im /etc-Verzeichnis, die mit "conf" enden: sudo cp /etc/*.conf /backup/

