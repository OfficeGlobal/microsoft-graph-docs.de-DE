---
title: Ressourcentyp oneDriveUsageAccountDetail
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 4b80ebc24aa45be0368dbb59d6d3e99e7adacc8c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063031"
---
# <a name="onedriveusageaccountdetail-resource-type"></a>Ressourcentyp oneDriveUsageAccountDetail

## <a name="properties"></a>Eigenschaften

| Eigenschaft                | Typ    |
| :---------------------- | :------ |
| reportRefreshDate       | Datum    |
| siteUrl                 | String  |
| ownerDisplayName        | String  |
| isDeleted               | Boolesch |
| lastActivityDate        | Datum    |
| fileCount               | Int64   |
| activeFileCount         | Int64   |
| storageUsedInBytes      | Int64   |
| storageAllocatedInBytes | Int64   |
| reportPeriod            | String  |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageAccountDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteUrl": "String", 
  "ownerDisplayName": "String", 
  "isDeleted": true, 
  "lastActivityDate": "Date", 
  "fileCount": 1024, 
  "activeFileCount": 1024, 
  "storageUsedInBytes": 1024, 
  "storageAllocatedInBytes": 1024, 
  "reportPeriod": "String"
}
```
