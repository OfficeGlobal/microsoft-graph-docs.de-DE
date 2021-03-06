---
title: Ressourcentyp emailActivityUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b871bf5dbaedd961fad09bf97be868f46e7430a1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938307"
---
# <a name="emailactivityuserdetail-resource-type"></a>Ressourcentyp emailActivityUserDetail

## <a name="properties"></a>Eigenschaften

| Eigenschaft          | Typ              |
| :---------------- | :---------------- |
| reportRefreshDate | Datum              |
| userPrincipalName | Zeichenfolge            |
| displayName       | Zeichenfolge            |
| isDeleted         | Boolescher Wert           |
| deletedDate       | Datum              |
| lastActivityDate  | Datum              |
| sendCount         | Int64             |
| receiveCount      | Int64             |
| readCount         | Int64             |
| assignedProducts  | Collection von Objekten des Typs „String“ |
| reportPeriod      | Zeichenfolge            |

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
