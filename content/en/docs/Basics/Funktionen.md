---
title: "Functions"
linkTitle: "Functions"
date: 2022-04-20
weight: 10
description: >
  PageJinn functions
---
We distinguish two phases when working with PageJinn. The editing phase and the planning phase.

### Editing Phase
In the editing phase, you open an existing issue to get an overview of the production status. You can check out any document by double-clicking (alternatively, by checking it out in the context menu or keyboard shortcut **a key**) on a page and then editing it in InDesign. As long as the document is checked out, a *green* check mark will appear on the pages of the document. (If a document is checked out by someone else, you'll see a *red* check mark).
After check-in, the new page view is displayed.

{{< alert title="Note" >}}The page PNG is generated by the client. It will be replaced later by the K4 database version.{{< /alert >}}

If you are working in standard workflow mode (in the config file *Advanced Workflow* is set to false), then the status of a document can also be changed from PageJinn. Click with pressed mouse button on the status bar of a page of the document and select another status. The status is changed via the K4 API. This function is not available in Advanced Workflow.


### Planning Phase
In the planning phase, you plan new issues, add new pages to an existing issue, delete or move pages. 
Every action you take in the planning phase results in the creation of new pages or a change in the page numbering of existing pages (for example, because pages are inserted).

PageJinn directly reflects the state after the action, for example, if you delete, the pages are taken out of view and the pagination in the status bar changes accordingly, but the pages of the document itself remain unchanged until you complete the planning phase and click **Execute** (alternatively **x key** for Execute). 

When you **Execute**, the current planning state is passed to the InDesign client, and there the pages are created, inserted, deleted, moved. When the action is complete, the newly created, or modified, issue is displayed in PageJinn. The pagination of the status bar and the actual pagination of the page are synchronized, and the PageJinn status in the icon bar is green again.


