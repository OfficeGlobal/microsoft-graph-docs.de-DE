---
title: reminder-Ressourcentyp
description: Eine Erinnerung für ein Ereignis in einem Benutzerkalender.
localization_priority: Normal
ms.openlocfilehash: a78c7f82ea0a7db9da45a60de98bb3b1311aaeeb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819964"
---
# <a name="reminder-resource-type"></a>reminder-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
|eventWebLink|String|Die URL zum Öfnen des Ereignisses in Outlook im Web.<br/><br/>Das Ereignis wird im Browser geöffnet, wenn Sie über Outlook im Web bei Ihrem Postfach angemeldet sind. Sie werden aufgefordert, sich anzumelden, wenn Sie noch nicht beim Browser angemeldet sind.<br/><br/>Auf diese URL kann von einem iFrame aus zugegriffen werden.|
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
<!-- {
  "type": "#page.annotation",
  "description": "reminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
