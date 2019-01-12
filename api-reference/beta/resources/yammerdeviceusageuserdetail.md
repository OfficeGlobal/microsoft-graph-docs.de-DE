---
title: Ressourcentyp yammerDeviceUsageUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 2b74222c1a636fac271268e228c8140e7d1cf33f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912008"
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
