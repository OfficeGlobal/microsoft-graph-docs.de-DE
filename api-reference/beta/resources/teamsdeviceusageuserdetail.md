---
title: Ressourcentyp teamsDeviceUsageUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
author: nkramer
ms.openlocfilehash: 1947b66a59190945e5a6b823b47ef8df7d02683a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329001"
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
