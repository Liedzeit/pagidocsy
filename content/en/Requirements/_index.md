---
title: "Requirements"
linkTitle: "Requirements"
weight: 2
description: >
  Requirements for working with PageJinn
---

{{% pageinfo %}}
**vjoon K4 ab Version 12**, Adobe InDesign 2020
{{% /pageinfo %}}

PageJinn is a module used for planning and managing K4 issues. Therefore, a prerequisite for working with it is that you are logged in to a K4 system.

We therefore assume that you are familiar with the [K4-System](https://vjoon.com/de/unser-angebot/ueberblick-k4/).

If you are not logged in to the  K4 System a message appears and PageJinn quits.

Internally, the PageJinn itself also logs on to the K4 system. (See [configuration file](/docs/configuration/config/): API User.) The internal K4 user communicates with K4 via the API. It loads the issue information and images. The creation of the pages happens on your client with your K4 account.




All pages displayed in PageJinn are png images of the relevant K4 pages. The images are downloaded directly from the K4 database via the API. The prerequisite is therefore that preview images of the pages are written in K4 at all. The images are rendered in the K4 system either by the InDesign server or by the client.

If in doubt, contact your K4 administrator.

For working with PageJinn we recommend creating pictures from the client, because then there is no delay in the display of the pages. (**MakeOnServer** = false)

![prefs](/images/k4Picprefs.png)







