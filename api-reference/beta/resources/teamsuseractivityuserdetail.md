---
title: Ressourcentyp teamsUserActivityUserDetail
description: Es folgt ein JSON-Darstellung der Ressource.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 2e3f64c7065343712f6a9d9c6a114bf95f24c171
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823653"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a>Ressourcentyp teamsUserActivityUserDetail

## <a name="properties"></a>Eigenschaften

| Eigenschaft                | Typ              |
| :---------------------- | :---------------- |
| reportRefreshDate       | Datum              |
| userPrincipalName       | String            |
| lastActivityDate        | Datum              |
| isDeleted               | Boolescher Wert           |
| deletedDate             | Datum              |
| assignedProducts        | Collection von Objekten des Typs „String“ |
| teamChatMessageCount    | Int64             |
| privateChatMessageCount | Int64             |
| callCount               | Int64             |
| meetingCount            | Int64             |
| hasOtherAction          | Boolescher Wert           |
| reportPeriod            | String            |

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
