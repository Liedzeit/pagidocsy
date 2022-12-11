---
title: "Konfigurationsdatei"
linkTitle: "Konfigurationsdatei"
date: 2017-01-05
weight: 3
description: >
  Beschreibung der Konfigurationsdatei.
---

 Bei der Installation von PageJinn wird automatisch eine Konfigurationsdatei angelegt. Die für die Funktionalität notwendigen Einträge können über die GUI vorgenommen werden. *Wenn* Sie diese Datei von Hand ändern, berücksichtigen Sie das json-Format.

{{< alert title="Tipp" >}}Laden Sie die config-Datei mit einem Browser wie Firefox, um sicher zu sein, dass sich kein Syntaxfehler eingeschlichen hat.{{< /alert >}}



**Beispiel für eine Konfigurationsdatei:**

```go
{
"PAGKEY":"U2FsdGVkX1854bQMq5zpFXrQkFabckQHKI/Z7Yv36fo=",
"DEBUG":true,
"APILog":true,
"hideAfterCheckout":false,
"advancedWorkFlow":true,
"LayoutNameWithPageRange":false,
"InDesign":"Adobe InDesign 2021",
"showLayoutNameInStatusBar":false,
"K4Version":"10",
"homeDir":"~/Documents/",
"bgColor":"#aabbcc",
"serverAddress":"http://127.0.0.1:9090/K4Server",
"apiuser":"PageJinn",
"apipw":"k4",
"apiremember":false,
"enableUserZoom":false,
"issueYearsToDisplayBeforeCurrent":"1",
"monthNames":["Januar","Februar","März","April","Mai","Juni","Juli","August","September","Oktober","November","Dezember"],
"dayNames":["Sonntag","Montag","Dienstag","Mittwoch","Donnerstag","Freitag","Sonnabend"],
"dueDateName":"Due Date",
"showDueDate":true,
"nameView":"name",
"NFR":false,
"1332490595545":
{"mdId":153,"mdType":2,"mdColor":"rgb(0,255,0)"}
}
```

| Konfig-Name            | Bedeutung           | Anmerkung
|-------------------|-----------------|------|
| PAGKEY   | Der Lizenzschlüssel, den Sie erhalten, wenn Sie PageJinn kaufen       |  |
| DEBUG            | Wenn dieser Wert auf *true* steht, wird eine Logdatei geschrieben    |
| APILog     | Logging der API-Funktionen  | 
| hideAfterCheckout     | Ausblenden des PageJinn-Fensters bei Checkout von Dokumenten  | im Moment deaktiviert
| advancedWorkFlow     | Ist der K4-Advanced Workflow für Layouts aktiv?  | 
| LayoutNameWithPageRange     | Der Seitenbereich wird mit in den Layoutnamen geschrieben | 
| InDesign     | Die verwendete InDesign-Version | 
| showLayoutNameInStatusBar     | Die verwendete InDesign-Version | 
| K4Version     | Die verwendete K4-Version | Nur für API-Funktionalität, alle Versionen ab Version 10 werden unterstützt
| homeDir     | Das Verzeichnis, in dem die PageJinn-Kundendaten liegen, u.a. die Konfigurationsdatei | 
| bgColor     | Die Hintergrundfarbe von PageJinn | 
| serverAddress     | Die URL des K4-Systems| 
| apiuser     | Ein K4-User mit Admin-Rechten | Dieser User muss Zugriffsrechte auf alle Publikationen haben, die mit PageJinn verwaltet werden sollen. | 
| apiremember     | Das Passwort für den apiuser |  |
| enableUserZoom     | User kann in Ausgabe ein- und auszoomen |  Wir empfehlen, diesen Wert auf *false* zu belassen |
| issueYearsToDisplayBeforeCurrent     | Die Anzahl der K4-Publikationsjahre vor dem aktuellen Jahr |  |
| monthNames     | Die Monatsnamen, die für den Header verwendet werden | im Moment deaktiviert | 
| dayNames     | Die Tagesnamen, die für den Header verwendet werden | im Moment deaktiviert | 
| dueDateName     | Das Passwort für den apiuser |  im Moment deaktiviert|
| nameView     | Dieser Eintrag bestimmt, welche Information im Statusbalken von PageJinn eingeblendet wird.| wird automatisch gesetzt|
| NFR     | Ist ein NFR-key vorhanden? | Nur zusammen mit einem gültigen NFR-Schlüssel wirksam. Schaltet zusätzliche noch im Test befindliche Funktionen frei.|
| 1332490595545     | K4-PublikationsId | Dieser Eintrag wird von PageJinn automatisch für jede verwendete Publikation erstellt. Darin sind intern verwendete Werte enthalten. Bitte nicht von Hand editieren! |


