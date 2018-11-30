---
title: Ressourcentyp skypeForBusinessPeerToPeerActivityUserCounts
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: ad3b409f3abc4cc9e7476825f9dbf5b7c2120d92
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063143"
---
# <a name="skypeforbusinesspeertopeeractivityusercounts-resource-type"></a>Ressourcentyp skypeForBusinessPeerToPeerActivityUserCounts

## <a name="properties"></a>Eigenschaften

| Eigenschaft          | Typ   |
| :---------------- | :----- |
| Instant Messaging                | Int64  |
| audio             | Int64  |
| video             | Int64  |
| appSharing        | Int64  |
| fileTransfer      | Int64  |
| reportRefreshDate | Datum   |
| reportDate        | Datum   |
| reportPeriod      | String |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityUserCounts"
} -->

```json
{
  "im": 1024, 
  "audio": 1024, 
  "video": 1024, 
  "appSharing": 1024, 
  "fileTransfer": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
