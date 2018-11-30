---
title: Ressourcentyp office365GroupsActivityCounts
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 4f3a5bf02f5f477ebab036fc9afa5d35a8061138
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064930"
---
# <a name="office365groupsactivitycounts-resource-type"></a>Ressourcentyp office365GroupsActivityCounts

## <a name="properties"></a>Eigenschaften

| Eigenschaft               | Typ   | Beschreibung                              |
| :--------------------- | :----- | ---------------------------------------- |
| reportRefreshDate      | Datum   | Das aktuelle Datum des Inhalts.          |
| exchangeEmailsReceived | Int64  | Die Anzahl von Postfächern Gruppe empfangenen e-Mails. |
| yammerMessagesPosted   | Int64  | Die Anzahl von Nachrichten zu Yammer-Gruppen bereitgestellt werden. |
| yammerMessagesRead     | Int64  | Lesen Sie die Anzahl der Nachrichten in Yammer-Gruppen. |
| yammerMessagesLiked    | Int64  | Die Anzahl der Nachrichten in Yammer-Gruppen gefallen. |
| reportDate             | Datum   | Das Datum, an dem eine Anzahl von e-Mails an eine Gruppenpostfach gesendet wurden, oder eine Anzahl von Nachrichten gesendet wurden, lesen oder in einer Gruppe Yammer gefallen |
| reportPeriod           | String | Die Anzahl der Tage, die der Bericht wird behandelt.    |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "exchangeEmailsReceived": 1024, 
  "yammerMessagesPosted": 1024, 
  "yammerMessagesRead": 1024, 
  "yammerMessagesLiked": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
