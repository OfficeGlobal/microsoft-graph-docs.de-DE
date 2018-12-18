---
title: Ressourcentyp teamsUserActivityUserDetail
description: Es folgt ein JSON-Darstellung der Ressource.
author: nkramer
ms.openlocfilehash: a1f47bc52c2a0a613598ce663f16023dce208c51
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331941"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a>Ressourcentyp teamsUserActivityUserDetail

## <a name="properties"></a>Eigenschaften

| Eigenschaft                | Typ              |
| :---------------------- | :---------------- |
| reportRefreshDate       | Datum              |
| userPrincipalName       | String            |
| lastActivityDate        | Datum              |
| isDeleted               | Boolesch           |
| deletedDate             | Datum              |
| assignedProducts        | Collection von Objekten des Typs „String“ |
| teamChatMessageCount    | Int64             |
| privateChatMessageCount | Int64             |
| callCount               | Int64             |
| meetingCount            | Int64             |
| hasOtherAction          | Boolesch           |
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
