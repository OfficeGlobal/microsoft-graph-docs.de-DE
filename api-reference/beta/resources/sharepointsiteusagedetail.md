---
title: Ressourcentyp sharePointSiteUsageDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: b555132b2cd70d3a01e0c80fe95f0b14417c61fa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861103"
---
# <a name="sharepointsiteusagedetail-resource-type"></a>Ressourcentyp sharePointSiteUsageDetail

## <a name="properties"></a>Eigenschaften

| Eigenschaft                | Typ    |
| :---------------------- | :------ |
| reportRefreshDate       | Datum    |
| siteId                  | Guid  |
| siteUrl                 | String  |
| ownerDisplayName        | String  |
| isDeleted               | Boolean |
| lastActivityDate        | Datum    |
| fileCount               | Int64   |
| activeFileCount         | Int64   |
| pageViewCount           | Int64   |
| visitedPageCount        | Int64   |
| storageUsedInBytes      | Int64   |
| storageAllocatedInBytes | Int64   |
| rootWebTemplate         | String  |
| reportPeriod            | String  |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointSiteUsageDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteId": "Guid", 
  "siteUrl": "String", 
  "ownerDisplayName": "String", 
  "isDeleted": true, 
  "lastActivityDate": "Date", 
  "fileCount": 1024, 
  "activeFileCount": 1024, 
  "pageViewCount": 1024, 
  "visitedPageCount": 1024, 
  "storageUsedInBytes": 1024, 
  "storageAllocatedInBytes": 1024, 
  "rootWebTemplate": "String", 
  "reportPeriod": "String"
}
```
