---
title: Ressourcentyp sharePointActivityUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a7dc324d821dca26ff1083f1e48c258e1955d72f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979943"
---
# <a name="sharepointactivityuserdetail-resource-type"></a>Ressourcentyp sharePointActivityUserDetail

## <a name="properties"></a>Eigenschaften

| Eigenschaft                  | Typ              |
| :------------------------ | :---------------- |
| reportRefreshDate         | Datum              |
| userPrincipalName         | Zeichenfolge            |
| isDeleted                 | Boolescher Wert           |
| deletedDate               | Datum              |
| lastActivityDate          | Datum              |
| viewedOrEditedFileCount   | Int64             |
| syncedFileCount           | Int64             |
| sharedInternallyFileCount | Int64             |
| sharedExternallyFileCount | Int64             |
| visitedPageCount          | Int64             |
| assignedProducts          | Collection von Objekten des Typs „String“ |
| reportPeriod              | Zeichenfolge            |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "lastActivityDate": "Date", 
  "viewedOrEditedFileCount": 1024, 
  "syncedFileCount": 1024, 
  "sharedInternallyFileCount": 1024, 
  "sharedExternallyFileCount": 1024, 
  "visitedPageCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
