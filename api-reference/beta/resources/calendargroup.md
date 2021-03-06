---
title: calendarGroup-Ressourcentyp
description: Eine Gruppe der Benutzerkalender.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: cea68da3a91396972c4e237d1fdaf0e16d65e3a3
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643713"
---
# <a name="calendargroup-resource-type"></a>calendarGroup-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Eine Gruppe der Benutzerkalender.

## <a name="methods"></a>Methoden

| Methode                                                      | Rückgabetyp                        | Beschreibung                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [Kalendergruppen auflisten](../api/user-list-calendargroups.md)  | [Kalendersammlung](calendar.md) | Dient zum Abrufen der Kalendergruppen des Benutzers.                               |
| [Kalendergruppe erstellen](../api/user-post-calendargroups.md) | [Kalender](calendar.md)            | Erstellt eine neue Kalendergruppe.                                  |
| [Kalendergruppe abrufen](../api/calendargroup-get.md)           | [calendarGroup](calendargroup.md)  | Dient zum Lesen der Eigenschaften und der Beziehungen eines Kalendergruppenobjekts. |
| [Update](../api/calendargroup-update.md)                    | [calendarGroup](calendargroup.md)  | Dient zum Aktualisieren des calendarGroup-Objekts.                                  |
| [Löschen](../api/calendargroup-delete.md)                    | Keine                               | Dient zum Löschen des calendarGroup-Objekts.                                  |
| [Kalender auflisten](../api/calendargroup-list-calendars.md)    | [Kalendersammlung](calendar.md) | Listet Kalender in einer Kalendergruppe auf.                           |
| [Kalender erstellen](../api/calendargroup-post-calendars.md)   | [Kalender](calendar.md)            | Erstellt einen neuen Kalender in einer Kalendergruppe.                    |

## <a name="properties"></a>Eigenschaften

| Eigenschaft  | Typ   | Beschreibung                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| name      | String | Der Gruppenname.                                                                                                                                                                                           |
| changeKey | String | Gibt die Version der Kalendergruppe an. Jedes Mal, wenn die Kalendergruppe geändert wird, wird auch ChangeKey geändert. Auf diese Weise kann Exchange Änderungen an der korrekten Version des Objekts vornehmen. Schreibgeschützt. |
| classId   | Guid   | Die Klassen-ID. Schreibgeschützt.                                                                                                                                                                          |
| id        | String | Eindeutiger Bezeichner für die Gruppe. Schreibgeschützt.                                                                                                                                                                 |

## <a name="relationships"></a>Beziehungen

| Beziehung | Typ                               | Beschreibung                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| Kalender    | [Kalendersammlung](calendar.md) | Die Kalender in Kalendergruppe. Navigation-Eigenschaft Schreibgeschützt. Lässt Nullwerte zu. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "calendars"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.calendarGroup"
}-->

```json
{
  "changeKey": "string",
  "classId": "guid",
  "id": "string (identifier)",
  "name": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "calendarGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/calendargroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
