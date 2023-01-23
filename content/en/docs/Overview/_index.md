---
title: "Overview"
linkTitle: "Overview"
weight: 1
description: >
 Here you will find everything from installation to daily work with PageJinn.
---



## What is PageJinn?

PageJinn is an Adobe CEP panel that lets you plan and create pages and page ranges in InDesign. 

CEP stands for Common Extensibility Platform. With it, Adobe provides a technology that third-party developers can use to create native panels. For you, this means you can use full page planning without leaving InDesign. The panel communicates directly with the host, which means you plan the pages and InDesign creates the new pages directly on your computer.

Double-click to open pages or page ranges, and the layout artist (or editor) works on the document as usual. When the document is closed, the new page views are immediately displayed, since the creation of the pages takes place on the client. (There might be a delay if you are using InDesign server.) At the same time, of course, the pages are written to the K4 database so that they are available to all team members.

### Function description

* Planning of any number of pages/page ranges directly in InDesign
* Assignment of InDesign master pages
* Loading of stored issue plans
* Creation of pages directly in the client (no InDesign server necessary)
* Moving, swapping, inserting and deleting pages and page sections
* Automatic repagination of all pages
* Double-page view mode 

### Integration with vjoon K4

* reading K4 issues via the K4 API
* Automatic check-in of generated pages
* Double-click checkout of K4 document directly from PageJinn
* No vjoon K4 object rules module required
* Change K4 status of documents via context menu (except in *Advanced Workflow* mode)


#### Restrictions

* **Is PageJinn suitable for you?** When adding, moving and deleting pages, all documents are checked out and processed. The prerequisite for this to work is that all documents are checked in. If you have a large number of people working on documents at the same time, it may be more advantageous for you to work with a pagination system that does not make the changes directly, but via the object rules, (which then also means that the changes are only realized when the object rules are applied to the individual clients). 

* Only InDesign layouts are edited with PageJinn. It does *not* create articles or ads.


* **What is PageJinn *not* suitable for?**: PageJinn works directly with the **k4** editorial system from **vjoon**. All data is read from and written to the K4 database. We are working on a version where optionally the data is kept locally and/or in a separate PageJinn database.