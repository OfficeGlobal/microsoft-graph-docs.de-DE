---
title: Ressourcentyp teamsDeviceUsageUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8cdd2fe1a212bb1d36846b80fc1b558c576deb47
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953785"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a>Ressourcentyp teamsDeviceUsageUserDetail

## <a name="properties"></a>Eigenschaften

| Eigenschaft          | Typ    |
| :---------------- | :------ |
| reportRefreshDate | Datum    |
| userPrincipalName | Zeichenfolge  |
| lastActivityDate  | Datum    |
| isDeleted         | Boolescher Wert |
| deletedDate       | Datum    |
| usedWeb           | Boolescher Wert |
| usedWindowsPhone  | Boolescher Wert |
| usediOS           | Boolescher Wert |
| usedMac           | Boolescher Wert |
| usedAndroidPhone  | Boolescher Wert |
| usedWindows       | Boolescher Wert |
| reportPeriod      | Zeichenfolge  |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "usedWeb": true, 
  "usedWindowsPhone": true, 
  "usediOS": true, 
  "usedMac": true, 
  "usedAndroidPhone": true, 
  "usedWindows": true, 
  "reportPeriod": "String"
}
```
