---
title: Ressourcentyp teamsUserActivityUserCounts
description: Es folgt eine JSON-Darstellung der Ressource.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 8a48a80992d8370a3b6b198862a3af901737fa04
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836659"
---
# <a name="teamsuseractivityusercounts-resource-type"></a>Ressourcentyp teamsUserActivityUserCounts

## <a name="properties"></a>Eigenschaften

| Eigenschaft            | Typ   |
| :------------------ | :----- |
| reportRefreshDate   | Datum   |
| reportDate          | Datum   |
| teamChatMessages    | Int64  |
| privateChatMessages | Int64  |
| Anrufe               | Int64  |
| Besprechungen            | Int64  |
| otherActions        | Int64  |
| reportPeriod        | Zeichenfolge |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "otherActions": 1024, 
  "reportPeriod": "String"
}
```
