
---
title: "Directories"
linkTitle: "Directories"
date: 222-04-13
description: >
 Where is PageJinn installed?
---

The actual PageJinn software is installed by the installer here:

`/Users/[username]/Library/Application\ Support/Adobe/CEP/Extensions/com.liedzeit.PAJ`.

The log file (if logging is enabled) can be found here:

`/Users/[username]/Documents/PageJinn/PageJinn.log`


In addition, PageJinn creates a directory **PageJinn** with all folders and files necessary for production. This directory is created in PageJinn's home directory (by default in the user's documents folder).

![structure](/images/structure.png)

Inside **PageJinn/PAJ** is PageJinn's configuration file and a folder for each publication used. Inside the publication folder PageJinn creates three subfolders, Master, Pics and Templates.

### Master

The master directory contains an InDesign template file (.indt) and a json file *templates.json* that describes the structure of the template file. 

{{< alert title="Note" >}}If not already present, create an InDesign template file in K4. (See [template file](/docs/configuration/template/)){{< /alert >}}

If no *.indt file* exists, PageJinn tries to find a file named "PageJinn" in the publication's template issue and copy it locally. The template.json file is created from this file. When creating the issue, PageJinn uses the Local .indt file (for performance reasons). The .json file is used by PageJinn to display the existing master pages in the GUI, as well as to read the size of the pages. You can modify both the local template file and the json file locally.

However, we recommend modifying the template within the K4 system. Next, click the **Update Template** button in PageJinn. This will rewrite the .indt and .json file

The structure of the json file looks like this:

```go
{
	"pageWidth":209.999999999936,
	"pageHeight":296.999999999461,
	"templates":[
		{
			"PageJinn [P]":[
				"A-Travel",
				"B-Politics"]
		}
	]
}
```

*PageWidth* and *pageHeight* are used by PageJinn to calculate the page sizes (aspect ratio). The entries under *PageJinn* stand for the *master pages* of the template. When you plan an issue with PageJinn, you assign a master page to each page, which is used when creating the output. At the same time, PageJinn attempts a mapping from master page to section. For this purpose the name part after the hyphen is used. I.e. if the master page is "A-Travel" and a section "Travel" exists within the publication, the document will be created in this section. If such a section does not exist, PageJinn uses the first section of the publication as a default.

The template used by PageJinn must have only one page (with Pagina 1).

{{< alert title="Note" >}}Only one template is supported at the moment, and it must be named "PageJinn".{{< /alert >}}


### Pics
The Pics directory contains the png files for each page. The images are loaded by PageJinn via API from the K4 database. When the document is modified, locally generated page images are temporarily used. 
In double page mode, PageJinn downloads a HiRes version of the image and places it in an appropriate directory.

### Templates
The templates directory contains the user-generated **plans** for issues to be created. These templates are also created in json format.