---
title: "Funktionen"
linkTitle: "Funktionen"
date: 2022-04-20
weight: 10
description: >
  Paginator-Funktionen
---
Wir unterscheiden zwei Phasen bei der Arbeit mit dem Paginator. Die Bearbeitungs- und die Planungsphase.

### Bearbeitungsphase
In der Bearbeitungsphase öffnen Sie eine vorhandene Ausgabe, um sich einen Überblick über den Stand der Produktion zu verschaffen. Sie können jedes Dokument durch Doppelklick (alternativ durch Auschecken im Kontext-Menü oder Tastaturküzel **a-Taste**) auf eine Seite auschecken und dann in InDesign bearbeiten. Solange das Dokument ausgecheckt ist, wird ein *grüner* Haken auf den Seiten des Dokuments eingeblendet. (Ist ein Dokument durch jemand anderen ausgecheckt, erkennen Sie das an einem *roten* Haken.)
Nach dem Einchecken wird die neue Seitenansicht angezeigt.

{{< alert >}}Das Seiten-PNG wird vom Client erzeugt. Es wird später durch die K4-Datenbankversion ersetzt.{{< /alert >}}

Wenn Sie im Standard-Workflowmodus arbeiten (in der Konfig-Datei steht *Advanced Workflow* auf false), dann lässt sich aus dem Paginator auch der Status eines Dokuments ändern. Klicken Sie mit gedrückter Maustaste auf die Statusleiste einer Seite des Dokuments und wählen Sie einen anderen Status. Der Status wird über die K4-API geändert. Diese Funktion steht im Advanced Workflow nicht zur Verfügung.


### Planungsphase
In der Planungsphase planen Sie neue Ausgaben, fügen in eine existierende Ausgabe neue Seiten hinzu, löschen oder verschieben Seiten. 
Jede Aktion, die Sie in der Planungsphase vornehmen, führt dazu, dass neue Seiten angelegt werden oder sich die Pagninierung von vorhandenen Seiten ändern soll (zum Beispiel weil Seiten eingefügt werden.)

Paginator spiegelt den Zustand nach der Aktion direkt wider, wenn Sie zum Beispiel löschen, werden die Seiten aus der Ansicht herausgenommen und die Paginierung in der Statusleiste ändert sich entsprechend, aber die Seiten des Dokuments selbst bleiben unverändert, solange bis Sie die Planungsphase abschließen und auf **Ausführen** (alternativ **x-Taste** für Execute) klicken. 

Wenn Sie **Ausführen**, wird der aktuelle Planungszustand an den InDesign-Client übergeben, und dort werden dann die Seiten erzeugt, eingefügt, gelöscht, verschoben. Ist die Aktion abgeschlossen, wird die neu angelegte, bzw. modifizierte, Ausgabe in Paginator angezeigt. Die Pagina der Statusleiste und die tatsächliche Pagina der Seite sind synchron, der Paginator-Status in der Icon-Leiste steht wieder auf Grün.


