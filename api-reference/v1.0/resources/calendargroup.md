---
title: calendarGroup-Ressourcentyp
description: Eine Gruppe der Benutzerkalender.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5b75ebf253276876129859be7d37ecb6748fc0d9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949626"
---
# <a name="calendargroup-resource-type"></a>calendarGroup-Ressourcentyp

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
| name      | Zeichenfolge | Der Gruppenname.                                                                                                                                                                                           |
| changeKey | Zeichenfolge | Gibt die Version der Kalendergruppe an. Jedes Mal, wenn die Kalendergruppe geändert wird, wird auch ChangeKey geändert. Auf diese Weise kann Exchange Änderungen an der korrekten Version des Objekts vornehmen. Schreibgeschützt. |
| classId   | Guid   | Die Klassen-ID. Schreibgeschützt.                                                                                                                                                                          |
| id        | Zeichenfolge | Eindeutiger Bezeichner für die Gruppe. Schreibgeschützt.                                                                                                                                                                 |

## <a name="relationships"></a>Beziehungen

| Beziehung | Typ                               | Beschreibung                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| Kalender    | [Kalendersammlung](calendar.md) | Die Kalender in Kalendergruppe. Navigation-Eigenschaft Schreibgeschützt. Lässt Nullwerte zu. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "calendars"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.calendarGroup",
  "@odata.annotations": [
    {
      "property": "calendars",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "navigability": "single",
        "searchable": false
      }
    }
  ]
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

<!-- {
  "type": "#page.annotation",
  "description": "calendarGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
