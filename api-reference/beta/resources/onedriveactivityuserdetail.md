---
title: Ressourcentyp oneDriveActivityUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: 2f498c7c9507c4210f12f76d57f62729f84da578
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820790"
---
# <a name="onedriveactivityuserdetail-resource-type"></a>Ressourcentyp oneDriveActivityUserDetail

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
| assignedProducts          | Collection von Objekten des Typs „String“ |
| reportPeriod              | String            |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveActivityUserDetail"
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
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
