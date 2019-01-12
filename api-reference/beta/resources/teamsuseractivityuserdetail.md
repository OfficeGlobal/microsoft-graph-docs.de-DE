---
title: Ressourcentyp teamsUserActivityUserDetail
description: Es folgt ein JSON-Darstellung der Ressource.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 32b611ee9ec01b0339389256b8c8dff9eac99fa9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913429"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a>Ressourcentyp teamsUserActivityUserDetail

## <a name="properties"></a>Eigenschaften

| Eigenschaft                | Typ              |
| :---------------------- | :---------------- |
| reportRefreshDate       | Datum              |
| userPrincipalName       | Zeichenfolge            |
| lastActivityDate        | Datum              |
| isDeleted               | Boolescher Wert           |
| deletedDate             | Datum              |
| assignedProducts        | Collection von Objekten des Typs „String“ |
| teamChatMessageCount    | Int64             |
| privateChatMessageCount | Int64             |
| callCount               | Int64             |
| meetingCount            | Int64             |
| hasOtherAction          | Boolescher Wert           |
| reportPeriod            | Zeichenfolge            |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt ein JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "assignedProducts": ["String"],
  "teamChatMessageCount": 1024, 
  "privateChatMessageCount": 1024, 
  "callCount": 1024, 
  "meetingCount": 1024, 
  "hasOtherAction": true, 
  "reportPeriod": "String"
}
```
