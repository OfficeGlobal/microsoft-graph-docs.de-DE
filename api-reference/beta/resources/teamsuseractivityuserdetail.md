---
title: Ressourcentyp teamsUserActivityUserDetail
description: Es folgt ein JSON-Darstellung der Ressource.
ms.openlocfilehash: 4e40ea4adf07450e6b51555df47579955a2a0286
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064811"
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
