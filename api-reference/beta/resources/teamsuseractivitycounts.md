---
title: Ressourcentyp teamsUserActivityCounts
description: Es folgt eine JSON-Darstellung der Ressource.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bcc0e9d1ed5c93c3d9f4ba97165d0413025a89cd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987524"
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
