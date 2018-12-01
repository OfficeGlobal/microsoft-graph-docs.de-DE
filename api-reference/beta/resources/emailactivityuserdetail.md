---
title: Ressourcentyp emailActivityUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 4f74b4af41c44e41b07bae1a8421011bc5188efc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058137"
---
# <a name="emailactivityuserdetail-resource-type"></a>Ressourcentyp emailActivityUserDetail

## <a name="properties"></a>Eigenschaften

| Eigenschaft          | Typ              |
| :---------------- | :---------------- |
| reportRefreshDate | Datum              |
| userPrincipalName | String            |
| displayName       | String            |
| isDeleted         | Boolesch           |
| deletedDate       | Datum              |
| lastActivityDate  | Datum              |
| sendCount         | Int64             |
| receiveCount      | Int64             |
| readCount         | Int64             |
| assignedProducts  | Collection von Objekten des Typs „String“ |
| reportPeriod      | String            |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "lastActivityDate": "Date", 
  "sendCount": 1024, 
  "receiveCount": 1024, 
  "readCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
