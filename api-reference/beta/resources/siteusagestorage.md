---
title: Ressourcentyp siteUsageStorage
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 1fdfa6cb2690d6dbacf5e534792061b6e64025d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059386"
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
