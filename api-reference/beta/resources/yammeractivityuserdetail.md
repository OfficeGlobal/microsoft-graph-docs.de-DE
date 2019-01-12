---
title: Ressourcentyp yammerActivityUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: d24e21c9525d49b7af5f8c4efaddd606c20c162b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923033"
---
# <a name="yammeractivityuserdetail-resource-type"></a>Ressourcentyp yammerActivityUserDetail

## <a name="properties"></a>Eigenschaften

| Eigenschaft          | Typ              |
| :---------------- | :---------------- |
| reportRefreshDate | Datum              |
| userPrincipalName | Zeichenfolge            |
| displayName       | Zeichenfolge            |
| userState         | Zeichenfolge            |
| stateChangeDate   | Datum              |
| lastActivityDate  | Datum              |
| postedCount       | Int64             |
| readCount         | Int64             |
| likedCount        | Int64             |
| assignedProducts  | Collection von Objekten des Typs „String“ |
| reportPeriod      | Zeichenfolge            |

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
