---
title: Ressourcentyp office365GroupsActivityFileCounts
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: 856bb4c74c8af35775b6fe71cb75d89935440bdb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819186"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a>Ressourcentyp office365GroupsActivityFileCounts

## <a name="properties"></a>Eigenschaften

| Eigenschaft          | Typ   | Beschreibung                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Datum   | Das aktuelle Datum des Inhalts.          |
| gesamt             | Int64  | Die Gesamtzahl der Dateien in der Gruppe SharePoint-Dokumentbibliothek. |
| aktive            | Int64  | Die Anzahl der Dateien, die angezeigt wurden, bearbeitet, freigegebene oder in der Gruppe SharePoint-Dokumentbibliothek synchronisiert. |
| reportDate        | Datum   | Das Datum, an dem eine Reihe von Dateien in der Gruppe SharePoint-Website aktiv waren. |
| reportPeriod      | String | Die Anzahl der Tage, die der Bericht wird behandelt.    |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {

  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityFileCounts"
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
