---
title: Ressourcentyp yammerDeviceUsageUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: 0f4d543ec8a96eaa4e237a1db1367efdc625c4e6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892015"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a>Ressourcentyp yammerDeviceUsageUserDetail

## <a name="properties"></a>Eigenschaften

| Eigenschaft          | Typ    |
| :---------------- | :------ |
| reportRefreshDate | Datum    |
| userPrincipalName | Zeichenfolge  |
| displayName       | Zeichenfolge  |
| userState         | Zeichenfolge  |
| stateChangeDate   | Datum    |
| lastActivityDate  | Datum    |
| usedWeb           | Boolescher Wert |
| usedWindowsPhone  | Boolescher Wert |
| usedAndroidPhone  | Boolescher Wert |
| usediPhone        | Boolescher Wert |
| usediPad          | Boolescher Wert |
| usedOthers        | Boolescher Wert |
| reportPeriod      | Zeichenfolge  |

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
