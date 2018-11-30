---
title: Ressourcentyp emailActivitySummary
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 039592a33cd004b9a5dc7800c0dbd4ece91bd48c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063550"
---
# <a name="emailactivitysummary-resource-type"></a>Ressourcentyp emailActivitySummary

## <a name="properties"></a>Eigenschaften

| Eigenschaft          | Typ   |
| :---------------- | :----- |
| reportRefreshDate | Datum   |
| Senden              | Int64  |
| empfangen           | Int64  |
| Lesen              | Int64  |
| reportDate        | Datum   |
| reportPeriod      | String |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "send": 1024, 
  "receive": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
