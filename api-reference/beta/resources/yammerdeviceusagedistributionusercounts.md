---
title: Ressourcentyp yammerDeviceUsageDistributionUserCounts
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 937691487046e2e77cc26b2c1f1a154966e1681b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936347"
---
# <a name="yammerdeviceusagedistributionusercounts-resource-type"></a>Ressourcentyp yammerDeviceUsageDistributionUserCounts

## <a name="properties"></a>Eigenschaften

| Eigenschaft          | Typ   |
| :---------------- | :----- |
| reportRefreshDate | Datum   |
| web               | Int32  |
| windowsPhone      | Int32  |
| androidPhone      | Int32  |
| iPhone            | Int32  |
| iPad              | Int32  |
| andere             | Int32  |
| reportPeriod      | Zeichenfolge |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerDeviceUsageDistributionUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "web": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "iPhone": 1024, 
  "iPad": 1024, 
  "other": 1024, 
  "reportPeriod": "String"
}
```
