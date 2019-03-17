---
title: shiftItem-Ressourcentyp
description: Ein shiftItem stellt eine Version der Schicht dar.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7ff829ca0f43124404b4b99b048c9919368b6009
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657707"
---
# <a name="shiftitem-resource-type"></a>shiftItem-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt eine Version einer [Schicht](shift.md)dar.

## <a name="properties"></a>Eigenschaften
| Eigenschaft                         | Typ                    | Beschreibung                                                                             |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| notes               | `string`                  | Die Hinweise für `shiftItem`.      |
| displayName               | `string`                  | Der Name des `shiftItem`. |
| startDateTime               | `DateTimeOffset`                  | Startdatum und-Uhrzeit für `shiftItem`. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Beispielsweise würde Mitternacht UTC am 1. Januar 2014 wie folgt aussehen: ' 2014-01-01T00:00:00Z '. Erforderlich. |
| endDateTime               | `DateTimeOffset`                  | Enddatum und-Uhrzeit für `shiftItem`. Erforderlich. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Beispielsweise würde Mitternacht UTC am 1. Januar 2014 wie folgt aussehen: ' 2014-01-01T00:00:00Z '. |
| theme | `enum`   |    |  |  | Unterstützte Farben: weiß; blau grün lila Rosa gelb grau DarkBlue Dunkelgrün DarkPurple darkPink; darkYellow. |
| Aktivitäten    | `collection([shiftActivity](shiftactivity.md))`    | Ein inkrementeller Teil einer Schicht, der Details darüber abdecken kann, wann und wo sich ein Mitarbeiter während seiner Schicht befindet. Zum Beispiel eine Zuordnung oder eine geplante Unterbrechung oder Mittagessen. Erforderlich. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shiftItem"
}-->
```json
{
  "displayName": "Day shift",
  "notes": "Please do inventory as part of your shift.",
  "startDateTime": "2019-03-11T15:00:00Z",
  "endDateTime": "2019-03-12T00:00:00Z",
  "theme": "blue",
  "activities": [
    {
      "isPaid": true,
      "startDateTime": "2019-03-11T15:00:00Z",
      "endDateTime": "2019-03-11T15:15:00Z",
      "code": "",
      "displayName": "Lunch"
    }
  ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shiftItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/shiftitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
