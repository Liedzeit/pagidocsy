---
title: "Template file"
linkTitle: "Template file"
date: 2022-10-09
weight: 3
description: >
  Creating a Template File
---

PageJinn requires access to an InDesign template file to display and create InDesign pages for each publication.

This template file (.indt) must be located locally in the PageJinn/PAJ directory. See [directories](/docs/installation/directories/)).

However, you should keep this file in the K4 system. Check in an InDesign file as a template named **PageJinn** into the K4 template issue. This file should contain only one page and should contain a sample page for each section you use. Also make sure that there are no missing fonts in this document.

If PageJinn does not find a local .indt file at startup, it will try to download the PageJinn template file from the K4 system. From the information in the file (height, width, sample pages), an additional *template.json* file is created 


{{< alert title="Attention" >}}If there is no local .indt file and there is none in the K4 system, the publications will not be displayed in PageJinn.{{< /alert >}}

If you subsequently change the K4 template file, for example to create new master pages, click **Update Template** in PageJinn afterwards.