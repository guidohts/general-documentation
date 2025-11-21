Die fiktive Elektro-Blitz GmbH aus Oberursel beschäftigt 25 Mitarbeiter.

Das Unternehmen verfügt über einen VDSL-Anschluss mit 250 MBit/s Downstream und 40 MBit/s Upstream. Dieser Anschluss
wurde realisiert mit einer Fritz!Box 7590. Alle Arbeitsplätze sind über LAN und WLAN mit dem Router verbunden. Es gibt auch noch ein ERP/CRM-System im selben Netz.
Er verwendet für das Intranet die Standardeinstellungen (192.168.178.0/24).

Das Unternehmen hat nun die Anforderung, eine Internetpräsenz (https://elektro-blitz-oberursel.de) aufzubauen. Das Hosting soll In-House erfolgen über den vorhandenen
VDSL-Zugang. Zunächst soll damit begonnen werden, statische Internetseiten zur Verfügung zu stellen. Dann ist es es geplant, einen Datenbankserver 
mit PostgreSQL aufzubauen und einen Application-Server (z.B. Tomcat). Dieser soll unter der URL https://elektro-blitz-oberursel.de/api verschiedene APIs anbieten.

Ein besonderes Augenmerk soll auf die Sicherheit gelegt werden.
Es ist sicherzustellen, dass mögliche Angriffe aus dem Internet unterbunden werden. Als zusätzliche Sicherheit muss gewährleistet sein, dass bei 
eventuell erfolgreichen Angriffen auf den Webserver von dort aus keine weitergehenden Zugriffe auf den Datenbankserver, auf das ERP/CRM-System und auf die
Arbeitsplätze möglich sind.

Wählen Sie die erforderliche Hard- und Software aus inklusive Betriebssystemen. Berücksichtigen Sie, dass der finanzielle Aufwand möglichst gering zu halten ist.
Planen Sie die Netzstruktur! Dokumentieren Sie alle geplanten Maßnahmen! Erstellen Sie ein Architektur- und Netzwerkschaubild!

Beschreiben Sie grob, wie die neuen Server installiert und später gewartet werden sollen!

Die Domain elektro-blitz-oberursel.de ist bei einem Registrar registriert, der auch den DNS-Server für diese Domain betreibt. Beschreiben Sie, welche DNS-Einträge 
erzeugt werden müssen! Für https wird ein Zertifikat benötigt. Beschreiben Sie, woher wir das bekommen!

