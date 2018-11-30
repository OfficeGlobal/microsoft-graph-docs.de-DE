---
title: Ressourcentyp skypeForBusinessOrganizerActivityMinuteCounts
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: f11d303bd8737d9fb2870042ee93557343d44a2f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064172"
---
# <a name="skypeforbusinessorganizeractivityminutecounts-resource-type"></a>Ressourcentyp skypeForBusinessOrganizerActivityMinuteCounts

## <a name="properties"></a>Eigenschaften

| Eigenschaft           | Typ   |
| :----------------- | :----- |
| audioVideo         | Int64  |
| dialInOut3rdParty  | Int64  |
| dialInOutMicrosoft | Int64  |
| reportRefreshDate  | Datum   |
| reportDate         | Datum   |
| reportPeriod       | String |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityMinuteCounts"
} -->

```json
{
  "audioVideo": 1024, 
  "dialInMicrosoft": 1024, 
  "dialOutMicrosoft": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
