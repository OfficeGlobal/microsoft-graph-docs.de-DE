---
title: Ressourcentyp yammerDeviceUsageDistributionUserCounts
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: ad8707d33c4200ea6729205819871d890929f001
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889033"
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
| reportPeriod      | String |

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
