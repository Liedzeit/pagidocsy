---
title: "Seiten einfügen"
linkTitle: "Seiten einfügen"
date: 2022-01-05
weight: 5
description: >
  Wie werden Seiten in die Ausgabe eingefügt?
---

### Seiten anlegen

Paginator ermöglicht das Anlegen von neuen Seiten auf zwei verschiedene Weisen.

Sie können Seiten innerhalb eines *vorhandenen* Dokuments anlgegen, dazu wählen Sie im Kontextmenü **Seiten einfügen**. Oder aber, Sie legen innerhalb der Ausgabe eine *neues* Dokument mit den neuen Seiten an. In diesem Fall wählen Sie im Kontextmenü **Seiten anfügen**.

![addPage](/images/addPage.png)

Wählen Sie die Anzahl der einzufügenden/anzufügenden Seiten, entweder über das Kontext-Untermenü (1-4 Seiten) oder über einen eingeblendeten Dialog, mit dem Sie beliebig viele Seiten anlegen können.

![addPage](/images/multiPages.png)

#### Seiten einfügen

Wenn Sie Seiten einfügen, zeigt Paginator die neuen Seiten mit dem Status des Parent-Dokumentes an.

![addPage](/images/insertPages.png)


Klicken Sie auf **Ausführen**, und Paginator legt in dem gewählten Dokument hinter der gewählten Seite die gewünschte Anzahl neuer Seiten an. Alle folgenden Dokumente erhalten die neue korrekte Pagina und werden gegebenenfalls umbenannt (wenn *LayoutNameWithPageRange* aktiv ist).


{{< alert title="Hinweis" >}}Bevor Sie eine Aktion ausführen, vergewissern Sie sich, dass alle Dokumente der Ausgabe eingecheckt sind, da Paginator sie auschecken können muss, um die Paginierung zu ändern.{{< /alert >}}

#### Seiten anfügen

Wenn Sie Seiten *anfügen*, haben die neuen Seiten in Paginator noch keine Statusfarbe. Die Seiten erhalten einen generischen Namen, und es wird ihnen standardmäßig die *erste* zur Verfügung stehende Musterseite zugewiesen.

Sie können nun über das Kontextmenü andere Musterseiten festlegen, und gegebenenfalls die Seiten *gruppieren* und *umbenennen*.



![addPages](/images/addPages.png)

Um die Seiten umzubenennen, klicken Sie in der Statusleiste auf den Namen. Die Statusleiste muss dazu den Namen anzeigen. Wird stattdessen die Musterseite angezeigt, wechseln Sie die Namensansicht mit **n-Taste**. Sind die Seiten gruppiert, brauchen Sie nur den Namen der ersten Seite zu ändern.

![renamePages](/images/renamePages.png)

{{< alert title="Hinweis" >}}Seiten anfügen ist nur am Ende einer Seitenstrecke möglich. Wenn Sie versuchen, Seiten innerhalb der Seitenstrecke anzulegen, erscheint eine entsprechende Fehlermeldung.{{< /alert >}}