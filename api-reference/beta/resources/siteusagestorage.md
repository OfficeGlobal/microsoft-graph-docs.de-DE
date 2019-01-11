---
title: Ressourcentyp siteUsageStorage
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: 1f656feacdbba3418049bd9f3072270aa04af798
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879926"
---
# <a name="siteusagestorage-resource-type"></a>Ressourcentyp siteUsageStorage

## <a name="properties"></a>Eigenschaften

| Eigenschaft           | Typ   |
| :----------------- | :----- |
| reportRefreshDate  | Datum   |
| Standorttyp           | String |
| storageUsedInBytes | Int64  |
| reportDate         | Datum   |
| reportPeriod       | String |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.siteUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "storageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
