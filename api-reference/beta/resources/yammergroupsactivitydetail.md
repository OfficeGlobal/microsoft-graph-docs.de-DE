---
title: Ressourcentyp yammerGroupsActivityDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c5b580f643686c27497fd24a6fe00c7750a6a938
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573263"
---
# <a name="yammergroupsactivitydetail-resource-type"></a>Ressourcentyp yammerGroupsActivityDetail

## <a name="properties"></a>Eigenschaften

| Eigenschaft           | Typ    |
| :----------------- | :------ |
| reportRefreshDate  | Date    |
| groupDisplayName   | String  |
| isDeleted          | Boolean |
| ownerPrincipalName | String  |
| lastActivityDate   | Date    |
| groupType          | String  |
| office365Connected | Boolean |
| memberCount        | Int64   |
| postedCount        | Int64   |
| readCount          | Int64   |
| likedCount         | Int64   |
| reportPeriod       | String  |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerGroupsActivityDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "groupDisplayName": "String", 
  "isDeleted": true, 
  "ownerPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "groupType": "String", 
  "office365Connected": true, 
  "memberCount": 1024, 
  "postedCount": 1024, 
  "readCount": 1024, 
  "likedCount": 1024, 
  "reportPeriod": "String"
}
```
