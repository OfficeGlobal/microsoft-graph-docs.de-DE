---
title: Ressourcentyp oneDriveActivityUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 29c9c8b723d4f87fa9858e26906878c973b37b09
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948247"
---
# <a name="onedriveactivityuserdetail-resource-type"></a>Ressourcentyp oneDriveActivityUserDetail

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
| assignedProducts          | Collection von Objekten des Typs „String“ |
| reportPeriod              | Zeichenfolge            |

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
