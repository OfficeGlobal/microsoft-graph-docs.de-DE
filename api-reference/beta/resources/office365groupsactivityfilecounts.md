---
title: Ressourcentyp office365GroupsActivityFileCounts
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: adff009d9047aa147c8042059fbdab8491288fb7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972558"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a>Ressourcentyp office365GroupsActivityFileCounts

## <a name="properties"></a>Eigenschaften

| Eigenschaft          | Typ   | Beschreibung                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Datum   | Das aktuelle Datum des Inhalts.          |
| gesamt             | Int64  | Die Gesamtzahl der Dateien in der Gruppe SharePoint-Dokumentbibliothek. |
| aktive            | Int64  | Die Anzahl der Dateien, die angezeigt wurden, bearbeitet, freigegebene oder in der Gruppe SharePoint-Dokumentbibliothek synchronisiert. |
| reportDate        | Datum   | Das Datum, an dem eine Reihe von Dateien in der Gruppe SharePoint-Website aktiv waren. |
| reportPeriod      | Zeichenfolge | Die Anzahl der Tage, die der Bericht wird behandelt.    |

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
