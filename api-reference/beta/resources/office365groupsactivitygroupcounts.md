---
title: Ressourcentyp office365GroupsActivityGroupCounts
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 12dc0121c8f37c694265fce0d6cb5f58e56e0966
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060833"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a>Ressourcentyp office365GroupsActivityGroupCounts

## <a name="properties"></a>Eigenschaften

| Eigenschaft          | Typ   | Beschreibung                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Datum   | Das aktuelle Datum des Inhalts.          |
| gesamt             | Int64  | Die Gesamtzahl der Gruppen.              |
| aktive            | Int64  | Die Anzahl der aktiven Gruppen. Eine Gruppe wird als aktiv betrachtet, wenn eines der folgenden aufgetreten ist: Postfach empfangene e-Mails; gruppieren Benutzer angezeigt, bearbeitet, freigegebene oder Dateien in SharePoint-Dokumentbibliothek synchronisiert; SharePoint-Seiten angezeigt; Benutzer gebucht, lesen oder gefallen Nachrichten in Yammer-Gruppen. |
| reportDate        | Datum   | Das Datum, an dem eine Anzahl von Gruppen aktiv waren. |
| reportPeriod      | String | Die Anzahl der Tage, die der Bericht wird behandelt.    |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityGroupCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
