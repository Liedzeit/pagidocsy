---
title: "Voraussetzungen"
linkTitle: "Voraussetzungen"
weight: 2
description: >
  Welche Voraussetzungen müssen für die Arbeit mit Paginator erfüllt sein?
---

{{% pageinfo %}}
**vjoon K4 ab Version 12**, Adobe Indesign 2020
{{% /pageinfo %}}

Paginator ist ein Modul, das für die Planung und Verwaltung von K4-Ausgaben eingesetzt wird. Voraussetzung für die Arbeit ist darum, dass Sie an einem K4-System angemeldet sind.

Wir gehen darum davon aus, dass Sie mit dem [K4-System](https://www.snap.de/produkte/workflow/vjoon-k4/) vertraut sind.

Wenn Sie nicht an einem K4-System angemeldet sind, erscheint eine entsprechende Meldung und Paginator beendet sich.

Intern meldet der Paginator selbst sich auch am K4-System an. (Siehe [Konfigarationsdatei](/docs/Konfigurationsdatei/): API-User.) Der interne K4-User kommuniziert über die API mit K4. Er lädt die Ausgabeninformationen und Bilder. Das Anlegen der Seiten geschieht auf Ihrem Client mit Ihrem K4-Account.




Alle im Paginator dargestellten Seiten sind png-Bilder der betreffenden K4-Seiten. Die Bilder werden direkt über die API aus der K4-Datenbank heruntergeladen. Voraussetzung ist darum, dass in K4 überhaupt Vorschaubilder der Seiten geschrieben werden. Die Bilder werden im K4-System entweder vom InDesign-Server berechnet oder vom Client.

Wenden Sie sich im Zweifelsfall an Ihren K4-Administrator.

Für die Arbeit mit Paginator empfehlen wir die Berechnung vom Client, da es dann bei der Darstellung der Seiten keine Verzögerung gibt. (**MakeOnServer** = false)

![prefs](/images/k4Picprefs.png)







