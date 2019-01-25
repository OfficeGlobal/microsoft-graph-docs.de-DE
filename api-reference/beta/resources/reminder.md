---
title: reminder-Ressourcentyp
description: Eine Erinnerung für ein Ereignis in einem Benutzerkalender.
localization_priority: Normal
ms.openlocfilehash: 88d9cb4f30f60819a606b3b1f3573d16860d9a00
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521033"
---
# <a name="reminder-resource-type"></a>reminder-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Eine Erinnerung für ein [Ereignis](event.md) in einem [Kalender](calendar.md)des Benutzers.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|changeKey|String|Gibt die Version der Erinnerung an. Jedes Mal, wenn die Erinnerung geändert wird, wird auch **changeKey** geändert. Auf diese Weise kann Exchange Änderungen an der korrekten Version des Objekts vornehmen.|
|eventEndTime|[DateTimeTimeZone](datetimetimezone.md)|Datum, Uhrzeit und Zeitzone für das Ende des Ereignisses.|
|eventId|String|Die eindeutige ID des Ereignisses. Schreibgeschützt.|
|eventLocation|[Location](location.md)|Der Speicherort des Ereignisses.|
|eventStartTime|[DateTimeTimeZone](datetimetimezone.md)|Datum, Uhrzeit und Zeitzone für den Beginn des Ereignisses.|
|eventSubject|String|Der Text der Betreffzeile des Ereignisses.|
|eventWebLink|Zeichenfolge|Die URL zum Öfnen des Ereignisses in Outlook im Web.<br/><br/>Das Ereignis wird im Browser geöffnet, wenn Sie über Outlook im Web bei Ihrem Postfach angemeldet sind. Sie werden aufgefordert, sich anzumelden, wenn Sie noch nicht beim Browser angemeldet sind.<br/><br/>Auf diese URL kann von einem iFrame aus zugegriffen werden.|
|reminderFireTime|[DateTimeTimeZone](datetimetimezone.md)|Datum, Uhrzeit und Zeitzone für das Ausführen der Erinnerung.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reminder"
}-->

```json
{
  "changeKey": "string",
  "eventEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "eventId": "string",
  "eventLocation": {"@odata.type": "microsoft.graph.location"},
  "eventStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "eventSubject": "string",
  "eventWebLink": "string",
  "reminderFireTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "reminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/reminder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
