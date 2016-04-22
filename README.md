#WIKIIMPORT
``Das Prüfsystem MEFOX ist für die interne Verwendung zur Kenngrößenerfassung, die Erstellung von Prüfprotokollen und Werkskalibrierscheinen von K1D und K3D an allen Sensorprüfplätzen der QM (Stand Oktober 2015) entwickelt worden. Alle zum Projekt gehörigen Dokumente (Auftrag, Erfassung IST-Zustand, Konzepte, Testdurchläufe, Ermittlung der Korrekturfaktoren, Zeitaufnamen,....) befinden sich unter "Z:\Software\Labview-Projekte\Projekt MEFOX". Ausserdem liegt dem Prüfwagen eine ausführliche Anleitung bei.``

## Anwenderdokumentation 

### *Komponenten*

####Messverstärker 

*wenn möglich FOTO einfügen*

*MV anhand der Nummerierung auf dem Foto erläutern*

####Zubehör 

*wenn möglich FOTO einfügen und erläutern*


### **Software**

#### Installation

Systemvoraussetzung: Windows XP Service Pack 3 oder höher

- Ordner "MEFOX-Installationsdatei" (Z:\Software\Labview-Projekte\Projekt MEFOX\MEFOX-Installationsdatei) auf lokalem PC kopieren
- darin enthaltene Odner "ME-Installer", dann "Volume" öffnen und Setup starten und den Anweisugen folgen
- Auf dem Desktop wird nun ein Ordner mit dem Name "MEFOX" erstellt, dain enthalten ist zum einen das Programm MEFOX sowie die dazugehörigen Konfigurationsdateien 
- nach Anschluss der Hardware den verwendeten COM-PORT über den Gerätemanager oder den Expertenmodus von MEFOX ermitteln und anschließend in der Konfigurationsdatei ändern. In der dritten Zeile bei: Arbeitsplatz="COM6" ist anstatt der 6 die Nummer des verwendeten COMPORTS einzutragen und die Datei abzuspeichern.
- Zusätzlich zur Installation der MEFOX-Software muss die Verbindung zur Datenbank über den ODBC-Server manuell eingerichtet werden. Die Installationsdatei "mysql-connector-odbc-5.3.4-win32.msi" befindet sich im zuvor lokal gespeicherten Ordner: MEFOX-Installationsdatei unter MEFOX-Anwendung\data

**Servereinstellungen**

- Servername: server
- Passwort: XXXXXXXX (bei Herr Bremsat erfragen)

<html>
<font color="red">'''Wichtig''': Von MEFOX generierte Daten werden '''NICHT''' lokal gespeichert. Die Verbindung zur Datenbank ist daher zwingend erforderlich!!!</font>
</html>

*wenn möglich FOTO einfügen*

### **Bedienung / Anwendung**

*wenn möglichen Screenshots einfügen und Funktionen erläutern*

### **Konfiguration / Änderung der Einstellungen**

Um Änderungen an den Voreinstellungen sowie den Inhalten der Dropdown-Menüs vornehmen zu können, ohne dies aufwendig im Quellcode tun zu müssen, wurden dafür Konfigurationsdateien angelegt, welche bei Programmstart ausgelesen werden. Es gibt vier verschiedene Konfigurationsdateien. Eine für die Einstellungsmöglichkeiten auf der Registerkarte „Auftragsdaten“, eine für die Registerkarte „Sensordaten“, eine für die Kommunikation mit der Datenbank sowie eine für die Systemkonfiguration. Diese befinden sich in dem bei der Installation erstellten Ordner "MEFOX" auf dem Desktop.
Sollten Änderungen an den Konfigurationsdateien vorgenommen oder diese ergänzt  werden muss sichergestellt werden, dass diese Änderungen Software und Datenbank konform sind. Abschließend muss in allen Konfigurationsdateien sowie in der Datenbank die Revisionsnummer aktualisiert werden. Dies dient zur Absicherung, dass sowohl die Datenbank als auch die Software mit den selben Parametern arbeitet.

Bsp.: Systemkonfigurationsdatei

In den eckigen Klammern stehen die Seriennummern der Messverstärker und darunter die Messverstärker spezifischen Korrekturfaktoren der einzelnen Kanäle, welche durch Testmessungen ermittelt wurden. Müssen diese auf Grund neuer Testmessungen geändert werden, so ist lediglich die grün markierte Zahl innerhalb der Anführungszeichen zu ändern und abzuspeichern. Bei Neustart der Software werden die neuen Korrekturfaktoren geladen.

[019CCE11]
;Widerstandskorrekturfaktor1
Widerstandskorrekturfaktor1="1,00113"
<html>
 <font color="green">1,00113</font>
</html>

### *Dokumentenerstellung*

Im Anschluss an die Messwerterfassung können die Daten über http://www.me-systeme.de oder http://me-systeme.de eingesehen und weiterverarbeitet werden.

Ansprechpartner http://brem: 
<html>
 <font color="orange">Herr Bremsat</font>
</html>

Ansprechpartner http:: 
<html>
 <font color="orange">Herr Kabelitz</font>
</html>

## Entwicklerdokumentation 

### **Software**

*Screenshot äußere Programmstruktur*

*Screenshot innere Programmstruktur*

### **Hardware**

Ansprechpartner:
<html>
 <font color="orange">Herr Schuldt</font>
</html>

:bangbang:

:+1:

![GitHub Logo](/images/logo.png)
Format: ![Alt Text](url)

- [x] 1. Aufgabe
- [x] 2. Aufgabe
- [x] 3. Aufgabe
- [ ] 4. Aufgabe

test
