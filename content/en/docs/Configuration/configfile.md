---
title: "Configuration File"
linkTitle: "Configuration File"
date: 2017-01-05
weight: 3
description: >
  Description of the Configuration File.
---

A configuration file is automatically created when PageJinn is installed. The entries necessary for functionality can be made via the GUI. *If* you change this file manually, consider the json format.

{{< alert title="Tip" >}}Load the config file with a browser like Firefox to be sure that no syntax error has crept in.{{< /alert >}}



**Example of a Configuration File:**

```go
{
"PAGKEY":"U2FsdGVkX1854bQMq5zpFXrQkFabckQHKI/Z7Yv36fo=",
"DEBUG":true,
"APILog":true,
"hideAfterCheckout":false,
"advancedWorkFlow":true,
"LayoutNameWithPageRange":false,
"InDesign":"Adobe InDesign 2021",
"showLayoutNameInStatusBar":false,
"K4Version":"10",
"homeDir":"~/Documents/",
"bgColor":"#aabbcc",
"serverAddress":"http://127.0.0.1:9090/K4Server",
"apiuser":"PageJinn",
"apipw":"k4",
"apiremember":false,
"enableUserZoom":false,
"issueYearsToDisplayBeforeCurrent":"1",
"monthNames":["Januar","Februar","März","April","Mai","Juni","Juli","August","September","Oktober","November","Dezember"],
"dayNames":["Sonntag","Montag","Dienstag","Mittwoch","Donnerstag","Freitag","Sonnabend"],
"dueDateName":"Due Date",
"showDueDate":true,
"nameView":"name",
"NFR":false,
"1332490595545":
{"mdId":153,"mdType":2,"mdColor":"rgb(0,255,0)"}
}
```

| Config name            | Meaning           | Note
|-------------------|-----------------|------|
| PAGKEY   | The license key you receive when you buy PageJinn      |  |
| DEBUG            | Set this to *true* to have PageJinn write a Log file    |
| APILog     | Logging of the API functions | 
| hideAfterCheckout     | Hides the PageJinn window after Check-Out of documents  | not currently active
| advancedWorkFlow     | Is K4 Advanced Workflow for Layouts active?  | 
| LayoutNameWithPageRange     | The page range will be written into the Layout name| 
| InDesign     | The used InDesign version | 
| showLayoutNameInStatusBar     | Should the name of the Layout be displayed | 
| K4Version     | The used K4 version | Only needed for API functions, all version starting from K4 10 are supported
| homeDir     | The folder with the PageJinn customer data including this config file | 
| bgColor     | The background color of PageJinn | 
| serverAddress     | The URL of the K4 System| 
| apiuser     | A K4 user with Admin rights | This User must have access rights for all  publications you want to manage with PageJinn | 
| apiremember     | The password for the apiuser |  |
| enableUserZoom     | Allow user to zoom in and out |  We recommend to leave this set to *false* |
| issueYearsToDisplayBeforeCurrent     | The number of years to go back from the current to display issues |  |
| monthNames     | The names of the months used in the header | currently deactivated | 
| dayNames     | The names of the week days used in the header | currently deactivated | 
| dueDateName     | The name for the dueDate |  currently deactivated|
| nameView     | This enty indicates which which information is displayed in the name field| set automatically by PageJinn|
| NFR     | Is there a NFR key? | This will bring up additional functions. You need a valid NFR key to use this|
| 1332490595545     | K4 publikation Id | This entry will be written by PageJinn automatically. Do not change it! |


