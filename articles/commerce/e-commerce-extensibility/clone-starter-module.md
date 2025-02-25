---
# required metadata

title: Clone a starter kit module
description: This topic describes how to clone a starter kit module.
author: samjarawan
manager: annbe
ms.date: 10/01/2019
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-retail
ms.technology: 

# optional metadata

# ms.search.form: 
audience: Developer
# ms.devlang: 
ms.reviewer: v-chgri
ms.search.scope: Retail, Core, Operations
# ms.tgt_pltfrm: 
ms.custom: 
ms.assetid: 
ms.search.region: Global
# ms.search.industry: 
ms.author: samjar
ms.search.validFrom: 2019-10-31
ms.dyn365.ops.version: Release 10.0.5

---
# Clone a starter kit module

[!include [banner](../includes/preview-banner.md)]
[!include [banner](../includes/banner.md)]

This topic describes how to clone a starter kit module.

## Overview

The Microsoft Dynamics 365 Commerce Online Software Development Kit (SDK) includes a set of starter kit modules that can be used on an e-Commerce site. Although these modules can't be modified directly, they can be cloned into new modules and then updated.

## Clone and update a module

To clone a module and then update it, use the **clone** command-line interface (CLI) command. When you run the below command, you replace **SDK\_MODULE\_NAME** with the name of the module that you want to modify and **NEW\_MODULE\_NAME** with the name of the new module.

**yarn msdyn365 clone SDK\_MODULE\_NAME NEW\_MODULE\_NAME**

This command adds the source code for the module to the /src/modules/ directory and pulls in any required dependencies for the module.

## Example

The following example shows how to clone the hero SDK module so that you can update it.

```
yarn msdyn365 clone hero heroExtended
```

It can take one to two minutes to clone the module. After the command has finished running, you can find the new module in the \\src\\modules\\ directory.

> [!NOTE]
> Module dependencies aren't automatically pulled down when you clone a module. Before you build the module, you must run Yarn and fix any missing dependencies.

## Preview a module

To preview the new module in a local web browser, follow these steps.

1. At a command prompt, go to your root SDK folder, and run the **yarn start** command. Here is an example.

    ```
    c:\repos\MyEcommerceSite\yarn start
    ```

2. In a web browser, open the following URL to view the module: `https://localhost:4000/modules?type=heroExtended`. Notice the module name in the **type=MODULE\_NAME** query string parameter.

You can now update the module code as needed.
