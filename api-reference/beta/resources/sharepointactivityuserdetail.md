---
title: Ressourcentyp sharePointActivityUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: 4503739a7b2e13cade72951ae56ab410f22608b9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880696"
---
# <a name="sharepointactivityuserdetail-resource-type"></a>Ressourcentyp sharePointActivityUserDetail

## <a name="properties"></a>Eigenschaften

| Eigenschaft                  | Typ              |
| :------------------------ | :---------------- |
| reportRefreshDate         | Datum              |
| userPrincipalName         | String            |
| isDeleted                 | Boolean           |
| deletedDate               | Datum              |
| lastActivityDate          | Datum              |
| viewedOrEditedFileCount   | Int64             |
| syncedFileCount           | Int64             |
| sharedInternallyFileCount | Int64             |
| sharedExternallyFileCount | Int64             |
| visitedPageCount          | Int64             |
| assignedProducts          | Collection von Objekten des Typs „String“ |
| reportPeriod              | String            |

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
