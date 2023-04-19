---
title: "Interface"
linkTitle: "Interface"
date: 2017-01-05
weight: 3
description: >
  The PageJinn interface.
---
After starting PageJinn you see this window.


![start](/images/start_e.png)
</br></br>

### Metadata
Under **Metadata**, select the K4 publication for which you want to edit or create issues.

Workflow contains the name for the K4 standard workflow for layouts *Layout*. 

Select an issue here. The number in the square bracket indicates how many pages the issue contains.

If the Metadata area is hidden, it can be shown by clicking the hamburger menu icon.

![This is an image](/images/auswahl.png)


**Update Template** updates the .indt file in PageJinn's master directory.

### Icon Bar

![refresh-Icon](/images/refresh-icon.png) reloads the active issue.

![edit-Icon](/images/edit-icon.png) shows and hides the edit bar.

![download-Icon](/images/download-icon.png) creates a PDF of the current issue and saves it to the download directory..

![prefs-Icon](/images/prefs-icon.png) shows and hides the preferences window.

![help-Icon](/images/help-icon.png) displays a window with short explanations and the keyboard shortcuts.

![status-Icon](/images/status-icon.png) shows the PageJinn status of the current issue. If it shows *yellow*, you should have the issue recalculated. If it shows *red*, you need to have the issue recalculated. (By clicking **Execute** in the edit bar).


### Issues View

![ausgabe](/images/ausgabe.png) 

If you have selected an issue with existing documents, PageJinn displays the entire issue scaled into the existing window space. PageJinn bases its output on the highest page number found. If there is no page for an underlying page number in the issue documents, the page is represented by blank pages (pages 2 and 3 in the figure).

If a page exists more than once, this is indicated by the warning bell. Click the bell to show the other page(s) with this page number (in this case 1).

#### Status Bar
The **status bar** shows the K4 status color of the document in question. The status bar shows the *name* of the document, or the *page number*. You can toggle the view by pressing the **n key**.

{{< alert >}}Make sure that the PageJinn has the **focus** when you use a keyboard shortcut.{{< /alert >}}

The border color indicates that pages belong to the same layout. Single-page documents do not have a frame. Show and hide the frames with **l key**.


#### Edit Bar
The **edit bar** contains a drop-down menu with the available *issue plans*, a button to save a new plan, as well as an input field, and a button to create new pages.

#### Views
PageJinn always displays the entire issue in the window at startup. If you enlarge or reduce the window, the display adjusts accordingly.

If *Allow UserZoom* is enabled in the preferences, you can also zoom in and out.

![Doulblepage-mode](/images/zoom.png) 


Reset (press the **r key**) to return to the default view.


##### Double page mode
Switch to *double page mode* by pressing the **d key**.
The pages that are under the mouse pointer will make up the entire window - and are replaced by a high-resolution version of the page image.

![Doulblepage-mode](/images/Doulblepage-mode.png) 




Navigate through the issue using the arrow keys.

{{< alert >}}In the double page mode some functions, for example those of the icon bar are deactivated.{{< /alert >}}

Switch to the normal view by pressing the **r key**.




