---
title: Ressourcentyp skypeForBusinessOrganizerActivityCounts
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 0729aef6367ebcb0a5edfaa461d80ffd8cb0775c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066162"
---
# <a name="skypeforbusinessorganizeractivitycounts-resource-type"></a>Ressourcentyp skypeForBusinessOrganizerActivityCounts

## <a name="properties"></a>Eigenschaften

| Eigenschaft           | Typ   |
| :----------------- | :----- |
| Instant Messaging                 | Int64  |
| audioVideo         | Int64  |
| appSharing         | Int64  |
| web                | Int64  |
| dialInOut3rdParty  | Int64  |
| dialInOutMicrosoft | Int64  |
| reportRefreshDate  | Datum   |
| reportDate         | Datum   |
| reportPeriod       | String |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityCounts"
} -->

```json
{
  "im": 1024, 
  "audioVideo": 1024, 
  "appSharing": 1024, 
  "web": 1024, 
  "dialInOut3rdParty": 1024, 
  "dialInOutMicrosoft": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
