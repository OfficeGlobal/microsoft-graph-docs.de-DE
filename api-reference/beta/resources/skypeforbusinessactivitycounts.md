---
title: Ressourcentyp skypeForBusinessActivityCounts
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 00c55df3a0a6201bd731938675880b9cbbe9cee6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064178"
---
# <a name="skypeforbusinessactivitycounts-resource-type"></a>Ressourcentyp skypeForBusinessActivityCounts

## <a name="properties"></a>Eigenschaften

| Eigenschaft          | Typ   |
| :---------------- | :----- |
| peerToPeer        | Int64  |
| organisiert         | Int64  |
| teilgenommen      | Int64  |
| reportRefreshDate | Datum   |
| reportDate        | Datum   |
| reportPeriod      | String |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessActivityCounts"
} -->

```json
{
  "peerToPeer": 1024, 
  "organized": 1024, 
  "participated": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
