---
title: Ressourcentyp yammerDeviceUsageUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 8812b61d974815fd1cdf1bbe1549a21193e5a2f4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065433"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a>Ressourcentyp yammerDeviceUsageUserDetail

## <a name="properties"></a>Eigenschaften

| Eigenschaft          | Typ    |
| :---------------- | :------ |
| reportRefreshDate | Datum    |
| userPrincipalName | String  |
| displayName       | String  |
| userState         | String  |
| stateChangeDate   | Datum    |
| lastActivityDate  | Datum    |
| usedWeb           | Boolesch |
| usedWindowsPhone  | Boolesch |
| usedAndroidPhone  | Boolesch |
| usediPhone        | Boolesch |
| usediPad          | Boolesch |
| usedOthers        | Boolesch |
| reportPeriod      | String  |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userState": "String", 
  "stateChangeDate": "Date", 
  "lastActivityDate": "Date", 
  "usedWeb": true, 
  "usedWindowsPhone": true, 
  "usedAndroidPhone": true, 
  "usediPhone": true, 
  "usediPad": true, 
  "usedOthers": true, 
  "reportPeriod": "String"
}
```
