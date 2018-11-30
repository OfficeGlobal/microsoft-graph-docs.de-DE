---
title: Ressourcentyp sharePointSiteUsageSiteCounts
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 631e01a417e177e356b701ca8dc93ffa51b4f50f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059782"
---
# <a name="sharepointsiteusagesitecounts-resource-type"></a>Ressourcentyp sharePointSiteUsageSiteCounts

## <a name="properties"></a>Eigenschaften

| Eigenschaft          | Typ   |
| :---------------- | :----- |
| reportRefreshDate | Datum   |
| Standorttyp          | String |
| gesamt             | Int64  |
| aktive            | Int64  |
| reportDate        | Datum   |
| reportPeriod      | String |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointSiteUsageSiteCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
