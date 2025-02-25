---
# required metadata

title: Item where used
description: This topic explains how to get an overview of where an item is used in Asset Management.
author: josaw1
manager: AnnBe
ms.date: 08/23/2019
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 

# optional metadata

ms.search.form: 
# ROBOTS: 
audience: Application User
# ms.devlang: 
ms.reviewer: josaw
ms.search.scope: Core, Operations
# ms.tgt_pltfrm: 
ms.custom: 
ms.assetid: 
ms.search.region: Global
# ms.search.industry: 
ms.author: mkirknel
ms.search.validFrom: 2019-08-31
ms.dyn365.ops.version: 10.0.5

---

# Item where used

[!include [banner](../../includes/banner.md)]

 

You can make a calculation for a specific item to get an overview of where in Asset Management the item has been used. The results show the context in which the item has been used during its lifetime. The **Item where used** page can be opened from the main Asset management menu, and it can also be accessed from the following pages:

[Asset BOM](../objects/object-BOM.md)

[Spare parts on asset type defaults](../setup-for-objects/object-types.md)

[Item forecast on Maintenance job type defaults forecast](../setup-for-work-orders/job-groups-and-job-types-variants-trades-and-checklists.md)

[Work order maintenance forecast](../work-orders/maintenance-forecasts.md)

[Work order purchase requisition](../work-orders/procurement.md)

[Work order purchase](../work-orders/procurement.md)

## Make an item-where-used calculation

1. Click **Asset management** > **Inquiries** > **Item where used**, or select the **Item where used** button on one of the pages mentioned above.

2. In the **Item where used** dialog, select the item for which you want to make the calculation in the **Item number** field.

3. You can use the **Level** field to indicate how detailed you want the item lines to be regarding functional locations. For example, if you insert the number "1" in the field, and you have a multi-level functional location structure, all item lines for a functional location will be shown on the top level. Therefore, relation/quantity on a line may be added up from functional locations located at a lower level. If you insert the number "0" in the **Level** field, you will see a detailed result showing all item lines on all the functional location levels to which they are related.

4. In the **Include** section, select "Yes" on the toggle buttons that you want to include in the calculation.

5. Click **OK** to start the calculation.

6. On the **Item where used** tab > **Group by...** action pane groups, select the relevant buttons to show the required detail level of the calculation. The selected action pane buttons are highlighted. Click on a button to activate or deactivate it.

7. If you want to show dimensions related to the item, click **Display dimensions**, and select the dimensions to be shown.

In the figure below, you see an example of an item-where-used calculation for item number "1000".

![Figure 1](media/12-controlling-and-reporting.png)

