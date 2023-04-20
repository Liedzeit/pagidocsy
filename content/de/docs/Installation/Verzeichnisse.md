
---
title: "Verzeichnisse"
linkTitle: "Verzeichnisse"
date: 222-04-13
description: >
 Wo wird PageJinn installiert?
---

Die eigentliche PageJinn-Software wird vom Installer hier installiert:

`/Users/[username]/Library/Application\ Support/Adobe/CEP/Extensions/com.snap.PAJ`

Die Logdatei (sofern das Logging eingeschaltet ist) finden Sie hier:

`//Users/[username]/Documents/PageJinn/PageJinn.log`


Daneben legt PageJinn ein Verzeichnis **PageJinn** mit allen für die Produktion notwendigen Ordnern und Dateien an. Dieses Verzeichnis wird im Home-Verzeichnis des PageJinns angelegt (standardmäßig im Dokumente-Ordner des Benutzers).

![struktur](/images/structure.png)

Innerhalb von **PageJinn/PAJ** befindet sich die Konfigurationsdatei von PageJinn und für jede verwendete Publikation ein Ordner. In dem Publikationsordner werden von PageJinn drei Unterordner angelegt, Master, Pics und Templates.

### Master

Das Master-Verzeichnis enthält eine InDesign-Vorlagedatei (Template) und eine json-Datei *templates.json*, die die Struktur der Vorlagedatei beschreibt. 

{{< alert title="Hinweis" >}}Wenn noch nicht vorhanden, legen Sie eine InDesign-Vorlagedatei in K4 an. (Siehe [Vorlagedatei](/docs/konfiguration/template/)){{< /alert >}}

Wenn keine *.indt-Datei* existiert, versucht PageJinn in der Templates-Ausgabe der Publikation eine Datei mit Namen "PageJinn" zu finden und lokal zu kopieren. Aus dieser Datei wird die template.json-Datei erzeugt. Beim Anlegen von Ausgaben benutzt PageJinn die Lokale .indt-Datei (aus Performance-Gründen). Die .json-Datei wird vom PageJinn benutzt, um in der GUI die vorhandenen Musterseiten anzuzeigen, sowie um die Größe der Seiten auszulesen. Sie können sowohl die lokale Template-Datei als auch die json-Datei lokal ändern.

Wir empfehlen aber, das Template innerhalb des K4-Systems zu modifizieren. Klicken Sie anschließend in PageJinn auf den **Voreinstellungen aktualisieren** Button. Damit werden .indt- und .json-Datei neu geschrieben

Die Struktur der json-Datei sieht so aus:

```go
{
	"pageWidth":209.999999999936,
	"pageHeight":296.999999999461,
	"templates":[
		{
			"PageJinn [P]":[
				"A-Travel",
				"B-Politics"]
		}
	]
}
```

*PageWidth* und *pageHeight* werden von PageJinn für die Berechnung der Seitengrößen (Aspect Ratio) benutzt. Die Einträge unter *PageJinn* stehen für die *Musterseiten* des Templates. Wenn Sie mit PageJinn eine Ausgabe planen, weisen Sie jeder Seite eine Musterseite zu, die beim Anlegen der Ausgabe verwendet wird. Gleichzeitig versucht PageJinn ein Mapping von Musterseite zu Ressort. Dazu wird der Namensteil nach dem Bindestrich verwendet. D.h. wenn innerhalb der Publikation ein Ressort "Travel" existiert, wird das Dokument mit diesem Ressort angelegt. Existiert ein solches Ressort nicht, verwendet PageJinn das erste Ressort der Publikation.

Das von PageJinn verwendete Template darf nur eine Seite haben (mit Pagina 1).

{{< alert title="Hinweis" >}}Im Moment wird nur ein Template unterstützt, das „PageJinn“ heißen muss.{{< /alert >}}


### Pics
Das Pics-Verzeichnis enthält die png-Dateien für jede Seite. Die Bilder werden von PageJinn per API aus der K4-Datenbank geladen. Bei Änderungen des Dokuments werden temporär lokal erzeugte Seitenbilder verwendet. 
Im Doppelseiten-Modus lädt PageJinn eine HiRes-Version des Bildes herunter und legt sie in einem entsprechenden Verzeichnis ab.

### Templates
Das Templates-Verzeichnis enthält die vom User erzeugten **Pläne** für anzulegende Ausgaben. Diese Templates werden ebenfalls im json-Format angelegt. 