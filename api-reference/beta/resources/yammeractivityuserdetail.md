---
title: Ressourcentyp yammerActivityUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: a1ca33efe8327b1c1e52de25714df9c0bd45ee05
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064132"
---
# <a name="yammeractivityuserdetail-resource-type"></a>Ressourcentyp yammerActivityUserDetail

## <a name="properties"></a>Eigenschaften

| Eigenschaft          | Typ              |
| :---------------- | :---------------- |
| reportRefreshDate | Datum              |
| userPrincipalName | String            |
| displayName       | String            |
| userState         | String            |
| stateChangeDate   | Datum              |
| lastActivityDate  | Datum              |
| postedCount       | Int64             |
| readCount         | Int64             |
| likedCount        | Int64             |
| assignedProducts  | Collection von Objekten des Typs „String“ |
| reportPeriod      | String            |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userState": "String", 
  "stateChangeDate": "Date", 
  "lastActivityDate": "Date", 
  "postedCount": 1024, 
  "readCount": 1024, 
  "likedCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
