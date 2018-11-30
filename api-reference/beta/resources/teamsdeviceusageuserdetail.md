---
title: Ressourcentyp teamsDeviceUsageUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 4eeec5f07a0a604249617ac87a62ea12b4052395
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065430"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a>Ressourcentyp teamsDeviceUsageUserDetail

## <a name="properties"></a>Eigenschaften

| Eigenschaft          | Typ    |
| :---------------- | :------ |
| reportRefreshDate | Datum    |
| userPrincipalName | String  |
| lastActivityDate  | Datum    |
| isDeleted         | Boolesch |
| deletedDate       | Datum    |
| usedWeb           | Boolesch |
| usedWindowsPhone  | Boolesch |
| usediOS           | Boolesch |
| usedMac           | Boolesch |
| usedAndroidPhone  | Boolesch |
| usedWindows       | Boolesch |
| reportPeriod      | String  |

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
