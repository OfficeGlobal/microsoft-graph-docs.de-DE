---
title: Ressourcentyp office365GroupsActivityGroupCounts
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: b202d5189c1edeeeaa45d447aa7cc078dd263858
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572486"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a>Ressourcentyp office365GroupsActivityGroupCounts

## <a name="properties"></a>Eigenschaften

| Eigenschaft          | Typ   | Beschreibung                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Date   | Das aktuelle Datum des Inhalts.          |
| gesamt             | Int64  | Die Gesamtzahl der Gruppen.              |
| aktive            | Int64  | Die Anzahl der aktiven Gruppen. Eine Gruppe wird als aktiv betrachtet, wenn eines der folgenden aufgetreten ist: Postfach empfangene e-Mails; gruppieren Benutzer angezeigt, bearbeitet, freigegebene oder Dateien in SharePoint-Dokumentbibliothek synchronisiert; SharePoint-Seiten angezeigt; Benutzer gebucht, lesen oder gefallen Nachrichten in Yammer-Gruppen. |
| reportDate        | Date   | Das Datum, an dem eine Anzahl von Gruppen aktiv waren. |
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
