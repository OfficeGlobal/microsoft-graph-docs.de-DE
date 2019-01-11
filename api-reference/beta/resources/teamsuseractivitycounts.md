---
title: Ressourcentyp teamsUserActivityCounts
description: Es folgt eine JSON-Darstellung der Ressource.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: c7351795f6b3dafbac996844fc1ac11cd24bbc03
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886590"
---
# <a name="teamsuseractivitycounts-resource-type"></a>Ressourcentyp teamsUserActivityCounts

## <a name="properties"></a>Eigenschaften

| Eigenschaft            | Typ   |
| :------------------ | :----- |
| reportRefreshDate   | Datum   |
| reportDate          | Datum   |
| teamChatMessages    | Int64  |
| privateChatMessages | Int64  |
| Anrufe               | Int64  |
| Besprechungen            | Int64  |
| reportPeriod        | Zeichenfolge |


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "reportPeriod": "String"
}
```
