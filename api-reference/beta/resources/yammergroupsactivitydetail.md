---
title: Ressourcentyp yammerGroupsActivityDetail
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 9a4bb00aecb2ae1d14b68a5388e0dedc7c41b1cb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059110"
---
# <a name="yammergroupsactivitydetail-resource-type"></a>Ressourcentyp yammerGroupsActivityDetail

## <a name="properties"></a>Eigenschaften

| Eigenschaft           | Typ    |
| :----------------- | :------ |
| reportRefreshDate  | Datum    |
| groupDisplayName   | String  |
| isDeleted          | Boolesch |
| ownerPrincipalName | String  |
| lastActivityDate   | Datum    |
| groupType          | String  |
| office365Connected | Boolesch |
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
