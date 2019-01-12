---
title: Ressourcentyp sharePointSiteUsageFileCounts
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1c88cd75e1b38da87042b7b67388ef869c15ec38
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950431"
---
# <a name="sharepointsiteusagefilecounts-resource-type"></a>Ressourcentyp sharePointSiteUsageFileCounts

## <a name="properties"></a>Eigenschaften

| Eigenschaft          | Typ   |
| :---------------- | :----- |
| reportRefreshDate | Datum   |
| Standorttyp          | Zeichenfolge |
| gesamt             | Int64  |
| aktive            | Int64  |
| reportDate        | Datum   |
| reportPeriod      | Zeichenfolge |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointSiteUsageFileCounts"
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
