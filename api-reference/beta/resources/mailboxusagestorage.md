---
title: Ressourcentyp mailboxUsageStorage
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 8cc26c5d3cc30529857ed3273f8ee66c7373327a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059837"
---
# <a name="mailboxusagestorage-resource-type"></a>Ressourcentyp mailboxUsageStorage

## <a name="properties"></a>Eigenschaften

| Eigenschaft           | Typ   |
| :----------------- | :----- |
| reportRefreshDate  | Datum   |
| storageUsedInBytes | Int64  |
| reportDate         | Datum   |
| reportPeriod       | String |

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
