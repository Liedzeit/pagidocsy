---
title: "Übersicht"
linkTitle: "Übersicht"
weight: -1
description: >
  Hier finden Sie alles von der Installation bis zur täglichen Arbeit mit dem Paginator.
---



## Was ist der Paginator?

Paginator ist ein Adobe-CEP-Panel, das Ihnen in InDesign das Planen und Anlegen von Seiten und Seitenstrecken erlaubt. 

CEP steht für Common Extensibility Platform. Damit stellt Adobe eine Technologie zur Verfügung, mit denen Drittentwickler native Panels erstellen können. Für Sie bedeutet das, dass Sie eine komplette Blattplanung verwenden können, ohne InDesign verlassen zu müssen. Das Panel kommuniziert direkt mit dem Host, das heißt, Sie planen die Seiten und InDesign legt direkt auf Ihrem Rechner die neuen Seiten an.

Per Doppelklick werden Seiten oder Seitenstrecken geöffnet und der Layouter (oder Redakteur) arbeitet wie gewohnt am Dokument. Beim Schließen werden sofort die neuen Seitenansichten angezeigt, da das Erzeugen der Seiten auf dem Client geschieht. Gleichzeitig werden die Seiten natürlich auch in die K4-Datenbank geschrieben, so dass sie allen Mitarbeitern im Team zur Verfügung stehen.

### Funktionsbeschreibung

* Planung von beliebig vielen Seiten/Seitenstrecken direkt in InDesign
* Zuweisung von Musterseiten
* Laden von hinterlegten Ausgabe-Plänen
* Erstellung der Seiten direkt im Client (kein InDesign-Server notwendig)
* Verschieben, Tauschen, Einfügen und Löschen von Seiten und Seitenstrecken
* Automatische Umpaginierung aller Seiten
* Doppelseitenansichts-Modus 

### Integration mit vjoon K4

* Auslesen der K4-Ausgaben über die K4-API
* automatisches Einchecken der erzeugten Seiten
* Auschecken von K4-Dokument direkt aus Paginator per Doppelklick
* Kein vjoon K4-Objektregeln-Modul notwendig
* Ändern des K4-Status von Dokumenten über Kontext-Menü (außer im *Advanced Workflow* Modus)


#### Einschränkungen

* **Ist Paginator geeignet für Sie?** Beim Hinzufügen, Verschieben und Löschen von Seiten werden alle Dokumente ausgecheckt und bearbeitet. Voraussetzung dafür, dass das funktioniert, ist, dass alle Dokumente eingecheckt sind. Wenn gleichzeitig sehr viele Mitarbeiter an den Dokumenten arbeiten, kann es für Sie vorteilhafter sein, mit einer Blattplanung zu arbeiten, die die Änderungen nicht direkt, sondern über die Objektregeln vornimmt, (was dann allerdings auch bedeutet, dass die Änderungen erst realsiert werden, wenn die Objektregeln auf den einzelnen Clients angewendet werden). 

* Mit Paginator werden nur InDesign-Layouts bearbeitet. Es werden *keine* Artikel oder Anzeigen angelegt.


* **Wofür eignet sich Paginator *noch* nicht?**: Paginator arbeitet direkt mit dem Redaktionssystem **k4** von **vjoon** zusammen. Alle Daten werden aus der K4-Datenbank gelesen und in sie geschrieben. Wir arbeiten an einer Version, in der optional die Daten lokal und/oder in einer eigenen Paginator-Datenbank gehalten werden.



