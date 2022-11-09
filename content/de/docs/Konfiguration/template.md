---
title: "Vorlagedatei"
linkTitle: "Vorlagedatei"
date: 2022-10-09
weight: 3
description: >
  Anlegen der Vorlagedatei
---

Paginator benötigt zur Darstellung und zum Anlegen von InDesign-Seiten für jede Publikation den Zugriff auf eine InDesign-Vorlagedatei.
Diese Vorlagedatei (.indt) muss lokal im SNAP-Verzeichnis liegen. Siehe [Verzeichnisse](/docs/installation/verzeichnisse/))

Sie sollten diese Datei allerdings im K4-System halten. Checken Sie eine InDesign-Datei als Vorlage mit dem Namen **Paginator** in die K4-Vorlage-Ausgabe (oder Templates-Ausgabe) ein. Diese Datei sollte nur eine Seite enthalten und für jedes von Ihnen verwendete Ressort ein Musterseite enthalten. Achten Sie auch darauf, dass es in diesem Dokument keine fehlenden Schriften gibt.

![Master-Pages](/images/master.png)


Wenn Paginator beim Start keine lokale .indt-Datei findet, wird versucht, die Paginator-Vorlagedatei aus dem K4-System herunterzuladen. Aus den Informationen der Datei (Höhe, Breite, Musterseiten) wird zusätzlich eine *template.json* Datei angelegt 


{{< alert title="Achtung" >}}Wenn keine lokale .indt-Datei vorhanden ist und sich auch keine im K4-System befindet, so werden die Publikationen im Paginator nicht angezeigt.{{< /alert >}}

Wenn Sie die K4-Vorlagedatei nachträglich ändern, zum Beispiel um neue Musterseiten anzulegen, klicken Sie anschließend im Paginator auf **Vorlage aktualisieren**.