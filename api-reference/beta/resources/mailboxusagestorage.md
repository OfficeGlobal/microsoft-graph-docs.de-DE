---
title: Ressourcentyp mailboxUsageStorage
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 44b97c7b18264e01c86b34bfd8265246f80ab031
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917867"
---
# <a name="mailboxusagestorage-resource-type"></a>Ressourcentyp mailboxUsageStorage

## <a name="properties"></a>Eigenschaften

| Eigenschaft           | Typ   |
| :----------------- | :----- |
| reportRefreshDate  | Datum   |
| storageUsedInBytes | Int64  |
| reportDate         | Datum   |
| reportPeriod       | Zeichenfolge |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "storageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
