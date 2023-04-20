---
title: "Insert Pages"
linkTitle: "Insert Pages"
date: 2022-01-05
weight: 5
description: >
  How to insert pages?
---

### Creating pages

PageJinn allows you to create new pages in two different ways.

You can create pages within an *existing* document by selecting **Insert Pages** from the context menu. Or, you can create a *new* document with the new pages within the K4 issue. In this case, choose **Add Pages** from the context menu.
<br>
<img src="/images/addPage_e.png" alt="deletePages" width="50%" height="50%">
<br>
Select the number of pages to insert/add, either from the context submenu (1-4 pages) or from a pop-up dialog that allows you to create as many pages as you want.



#### Insert pages

When you insert pages, PageJinn displays the new pages with the status of the parent document.

![addPage](/images/insertPages.png)


Click **Execute**, and PageJinn creates the desired number of new pages in the selected document after the selected page. All following documents get the new correct pagination and are renamed if necessary (if *LayoutNameWithPageRange* is active).

{{< alert title="Note" >}}Before performing any action, make sure that all documents in the issue are checked in, since PageJinn must be able to check them out in order to change the pagination.{{< /alert >}}

#### Add pages

When you *add* pages, the new pages do not yet have a status color in PageJinn. The pages are given a generic name, and they are assigned the *first* available master page by default.

You can now specify other master pages via the context menu, and *group* and *rename* the pages if necessary.



![addPages](/images/addPages_e.png)

To rename the pages, click the name in the status bar. The status bar must display the name for this. If the sample page is displayed instead, change the name view with **n key**. If the pages are grouped, you only need to change the name of the first page.

![renamePages](/images/renamePages.png)

{{< alert title="Note" >}}Adding pages is only possible at the end of a page section. If you try to create pages within the page range, a corresponding error message appears.{{< /alert >}}