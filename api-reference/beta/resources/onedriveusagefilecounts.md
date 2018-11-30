---
title: Ressourcentyp oneDriveUsageFileCounts
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 98e387b97687a4aab55e8d94e72fdbfa585a0e84
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059050"
---
# <a name="onedriveusagefilecounts-resource-type"></a>Ressourcentyp oneDriveUsageFileCounts

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
  "@odata.type": "microsoft.graph.oneDriveUsageFileCounts"
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
