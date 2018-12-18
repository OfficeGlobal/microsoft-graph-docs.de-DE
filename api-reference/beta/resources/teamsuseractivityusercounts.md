---
title: Ressourcentyp teamsUserActivityUserCounts
description: Es folgt eine JSON-Darstellung der Ressource.
author: nkramer
ms.openlocfilehash: f4e10f1e34d4c6bdbed83279b98632c504630bc7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330457"
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
| reportPeriod        | String |

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
