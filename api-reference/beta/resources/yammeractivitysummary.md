---
title: Ressourcentyp yammerActivitySummary
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 6ff2b347de77f91c96cb5f5be797eb70db0bbbee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059099"
---
# <a name="yammeractivitysummary-resource-type"></a>Ressourcentyp yammerActivitySummary

## <a name="properties"></a>Eigenschaften

| Eigenschaft          | Typ   |
| :---------------- | :----- |
| reportRefreshDate | Datum   |
| gefallen             | Int64  |
| gebucht            | Int64  |
| Lesen              | Int64  |
| reportDate        | Datum   |
| reportPeriod      | String |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "liked": 1024, 
  "posted": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
