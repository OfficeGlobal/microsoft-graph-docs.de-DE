---
title: Ressourcentyp teamsUserActivityCounts
description: Es folgt eine JSON-Darstellung der Ressource.
author: nkramer
ms.openlocfilehash: f67540f4172993b1076d9590438262b0d4da1846
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334517"
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
| reportPeriod        | String |


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
