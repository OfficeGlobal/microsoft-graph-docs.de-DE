---
title: Ressourcentyp emailAppUsageVersionsUserCounts
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: 2aff22c0ae1d3042859f3457f398ef5d0a5ffbe7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884847"
---
# <a name="emailappusageversionsusercounts-resource-type"></a>Ressourcentyp emailAppUsageVersionsUserCounts

## <a name="properties"></a>Eigenschaften

| Eigenschaft          | Typ   |
| :---------------- | :----- |
| reportRefreshDate | Datum   |
| outlook2016       | Int64  |
| outlook2013       | Int64  |
| outlook2010       | Int64  |
| outlook2007       | Int64  |
| unbestimmten      | Int64  |
| reportPeriod      | Zeichenfolge |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageVersionsUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "outlook2016": 1024, 
  "outlook2013": 1024, 
  "outlook2010": 1024, 
  "outlook2007": 1024, 
  "undetermined": 1024, 
  "reportPeriod": "String"
}
```
