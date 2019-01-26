---
title: Ressourcentyp office365GroupsActivityCounts
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c94e79f688e117960b3a8a0f2c9888a908634a82
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572332"
---
# <a name="office365groupsactivitycounts-resource-type"></a>Ressourcentyp office365GroupsActivityCounts

## <a name="properties"></a>Eigenschaften

| Eigenschaft               | Typ   | Beschreibung                              |
| :--------------------- | :----- | ---------------------------------------- |
| reportRefreshDate      | Date   | Das aktuelle Datum des Inhalts.          |
| exchangeEmailsReceived | Int64  | Die Anzahl von Postfächern Gruppe empfangenen e-Mails. |
| yammerMessagesPosted   | Int64  | Die Anzahl von Nachrichten zu Yammer-Gruppen bereitgestellt werden. |
| yammerMessagesRead     | Int64  | Lesen Sie die Anzahl der Nachrichten in Yammer-Gruppen. |
| yammerMessagesLiked    | Int64  | Die Anzahl der Nachrichten in Yammer-Gruppen gefallen. |
| reportDate             | Date   | Das Datum, an dem eine Anzahl von e-Mails an eine Gruppenpostfach gesendet wurden, oder eine Anzahl von Nachrichten gesendet wurden, lesen oder in einer Gruppe Yammer gefallen |
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
