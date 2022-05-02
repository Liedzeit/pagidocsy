---
title: "Neue Ausgabe"
linkTitle: "Neue Ausgabe"
date: 2017-01-05
weight: 1
description: >
  Anlegen einer neue Ausgabe.
---

### Ausgabe planen
Die Planung und Erzeugung einer neuen Ausgabe ist die Kernfunktion von Paginator.

{{< alert title="Hinweis" >}}Paginator erstellt Dokumente *innerhalb* einer K4-Ausgabe. Das Anlegen der K4-Ausgabe muss im Admin von K4 geschehen.{{< /alert >}}



Wählen Sie unter *Metadata* eine leere Ausgabe (in den eckigen Klammern befindet sich eine 0).

![cnoosenewIssue](/images/choosenewissue.png)


Geben Sie an wieviele Seiten die Ausgaben enthalten soll und klicken Sie auf **Seiten anlegen**.

<br>

![emptyIssue](/images/emptyIssue.png)


Paginator legt die Seiten an. Jede Seite erhält einen generischen Namen bestehend aus dem Namen der Ausgabe und einer durchlaufenden Seitennummer.

<br>

![newIssue](/images/newIssue.png)


Wählen Sie nun für jede Seite oder einen gewählten Seitenbereich aus dem Kontext-Menü eine Musterseite aus. Sie können einen Seitenbereich, wie üblich, durch Anklicken mit gedrückter Shift- oder Befehlstaste selektieren. Selektierte Seiten werden mit einem blauen Rahmen dargestellt.

{{< alert title="Hinweis" >}}Nur zusammenhängende Seiten können einen Seitenbereich bilden.{{< /alert >}}



![newIssue](/images/kontext.png)


Um einen Seitenbereich zu definieren, aus dem *ein* Dokument werden soll, wählen Sie im Kontext-Menü **Gruppieren** (alternativ **g-Taste**).

Gruppierte Seiten erhalten einen farbigen Rahmen (ein- und ausblendbar mit **l-Taste**). In der Statusleiste steht die Seitennummer und das Kürzel für die gewählte Musterseite.

![plan](/images/plan.png)



Sie können einzelnen Seiten oder Seitenstrecken einen eigenen Namen zuweisen. Wechseln Sie mit **n-Taste** in die Namensansicht und fahren Sie mit der Maus über den Namen. Geben Sie nun einen eigenen Namen für die Seite oder die Seitenstrecke ein. 

![changeName](/images/changeName.png)


### Plan sichern

Um die Schritte der Planung abzukürzen, ist es möglich den Plan, wie er jetzt besteht, also **vor** dem Ausführen zu sichern.
Klicken Sie auf **Plan sichern**.

Geben Sie im Dialog einen Namen für Ihren Plan ein. Dieser Plan steht Ihnen im Auswahlmenü bei der nächsten Planung zur Verfügung. Anstatt neue Seiten zu planen, rufen Sie dann den Plan auf, und modifizieren gegebenenfalls die zugewiesenen Musterseiten.

{{< alert title="Hinweis" >}}Ändern Sie nicht den Speicherplatz, da Paginator beim Start die hier hinterlegten Template-Pläne ausliest.{{< /alert >}}

![changeName](/images/savePlan.png)



### Ausgabe erzeugen

Klicken Sie auf **Ausführen**, um den Prozess der Ausgabenerzeugung zu starten.

![changeName](/images/process.png)
