---
title: "Troubleshooting"
description: 
author: asb3993
ms.author: amburns
ms.date: 04/14/2017
ms.topic: article
ms.assetid: CE860D79-E29E-4B93-B094-BE74B35FC1C2
---

# Troubleshooting

## Viewing Logs in Visual Studio for Mac
 
Logs can be found by browsing to the **Help > Open Log Directory** menu item, as illustrated below:

![Open Log directory menu item](media/troubleshooting-image1.png)

## Viewing Exceptions

When an exception has been caught, an exception bubble will appear. To view more details, select the **View Details** button:

![View more details about an exception](media/troubleshooting-image2.png)

This will the display Show Details dialog, providing more information regarding the exception:

![](media/troubleshooting-image3.png)

Important sections of the dialog, which are numbered above are described in detail below:

1. The exception type, which shows the full name of the exception type that is being observed.
2. The exception message, which shows the value of the Message property of the exception object.
3. The Inner exception type, which shows the full name of the exception type for the currently selected exception in the Inner exception tree view.
4. The Inner exception message, shows the value of the Message property of the selected exception in Inner exception tree view.
5. Stacktrace view. This can be collapsed via a disclosure arrow and contains stack frames entries.
6. Example of non-user code entries.
7. Example of user code entries.
8. Properties view, which shows all properties and fields of the exception. This can be collapsed via a disclosure arrow.
9. Inner exception tree view. Select inner exceptions in this view via keyboard up/down arrows or with the mouse or trackpad.
10. By default, this is set to what the **Debug project code only** option in debugger settings is set. Selecting this box will enable all non-user code to collapse into one line in the stacktrace.
11. A copy button to copy the `exception.ToString()` output to clipboard.

Note that some of these sections will only be visible when exception has an inner exception.