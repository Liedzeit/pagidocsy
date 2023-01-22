---
title: "Requirements"
linkTitle: "Requirements"
weight: 2
description: >
  Requirements for working with PageJinn
---

{{% pageinfo %}}
**vjoon K4 ab Version 12**, Adobe InDesign 2020
{{% /pageinfo %}}

PageJinn is a module used for planning and managing K4 outputs. Therefore, a prerequisite for working with it is that you are logged in to a K4 system.

We therefore assume that you are familiar with the [K4-System](https://vjoon.com/de/unser-angebot/ueberblick-k4/).

If you are not logged in to the  K4 System a message appears and PageJinn quits.

Intern meldet der PageJinn selbst sich auch am K4-System an. (Siehe [Konfigurationsdatei](/docs/konfiguration/config/): API-User.) Der interne K4-User kommuniziert über die API mit K4. Er lädt die Ausgabeninformationen und Bilder. Das Anlegen der Seiten geschieht auf Ihrem Client mit Ihrem K4-Account.




Alle im PageJinn dargestellten Seiten sind png-Bilder der betreffenden K4-Seiten. Die Bilder werden direkt über die API aus der K4-Datenbank heruntergeladen. Voraussetzung ist darum, dass in K4 überhaupt Vorschaubilder der Seiten geschrieben werden. Die Bilder werden im K4-System entweder vom InDesign-Server berechnet oder vom Client.

Wenden Sie sich im Zweifelsfall an Ihren K4-Administrator.

Für die Arbeit mit PageJinn empfehlen wir die Berechnung vom Client, da es dann bei der Darstellung der Seiten keine Verzögerung gibt. (**MakeOnServer** = false)

![prefs](/images/k4Picprefs.png)







