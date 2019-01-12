---
title: Ressourcentyp yammerGroupsActivityDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 79ce924fff5d1ce9ca861c3d48589a0ecad149dc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939168"
---
# <a name="yammergroupsactivitydetail-resource-type"></a>Ressourcentyp yammerGroupsActivityDetail

## <a name="properties"></a>Eigenschaften

| Eigenschaft           | Typ    |
| :----------------- | :------ |
| reportRefreshDate  | Datum    |
| groupDisplayName   | Zeichenfolge  |
| isDeleted          | Boolescher Wert |
| ownerPrincipalName | Zeichenfolge  |
| lastActivityDate   | Datum    |
| groupType          | Zeichenfolge  |
| office365Connected | Boolescher Wert |
| memberCount        | Int64   |
| postedCount        | Int64   |
| readCount          | Int64   |
| likedCount         | Int64   |
| reportPeriod       | Zeichenfolge  |

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
