---
title: Ressourcentyp skypeForBusinessDeviceUsageUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: b62920d124fd52e0f653c128eeb0956cdfe0c680
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059714"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a>Ressourcentyp skypeForBusinessDeviceUsageUserDetail

## <a name="properties"></a>Eigenschaften

| Eigenschaft          | Typ    |
| :---------------- | :------ |
| reportRefreshDate | Datum    |
| userPrincipalName | String  |
| lastActivityDate  | Datum    |
| usedWindows       | Boolesch |
| usedWindowsPhone  | Boolesch |
| usedAndroidPhone  | Boolesch |
| usediPhone        | Boolesch |
| usediPad          | Boolesch |
| reportPeriod      | String  |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "usedWindows": true, 
  "usedWindowsPhone": true, 
  "usedAndroidPhone": true, 
  "usediPhone": true, 
  "usediPad": true, 
  "reportPeriod": "String"
}
```
