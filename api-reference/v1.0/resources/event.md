---
title: Ressourcentyp „event“
description: Ein Ereignis in einem Kalender
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 5288087a5288f31903dcc25fd4ef186c1bcf8783
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990810"
---
# <a name="event-resource-type"></a>Ressourcentyp „event“

Ein Ereignis in einem Kalender des [Benutzers](user.md) oder Standardkalender einer Office 365- [Gruppe](group.md).

Diese Ressource unterstützt Folgendes:

- Hinzufügen von Ihren eigenen Daten zu benutzerdefinierten Eigenschaften als [Extensions](/graph/extensibility-overview).
- Abonnieren von [Benachrichtigungen zu ändern](/graph/webhooks).
- Verwenden einer [Delta-Abfrage](/graph/delta-query-overview) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen der [delta](../api/event-delta.md)-Funktion.

> **Hinweis:** Es gibt einige kleinere Unterschiede bei der Verarbeitung von Benutzerkalender, Gruppenkalender und deren Ereignisse interagieren können:

 - Sie können nur Benutzerkalender in einer [CalendarGroup](calendargroup.md)organisieren.
 - Outlook akzeptiert automatisch alle Besprechungsanfragen für Gruppen. Sie können für Kalender nur _Benutzer_ [annehmen](../api/event-accept.md), [mit Vorbehalt annehmen](../api/event-tentativelyaccept.md)oder [Ablehnen](../api/event-decline.md) von Besprechungsanfragen.
  - Outlook unterstützt keine Erinnerungen für Ereignisse gruppieren. Sie können für _Benutzer_ Kalender nur [erneut erinnern](../api/event-snoozereminder.md) oder eine [Erinnerung](reminder.md) [zu schließen](../api/event-dismissreminder.md) .

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[List events](../api/user-list-events.md)|[Ereignissammlung](event.md) |Ruft eine Liste der [event](../resources/event.md)-Objekte im Postfach des Benutzers ab. Die Liste enthält einzelne Instanzen von Besprechungen und Serienmaster.|
|[Ereignis erstellen](../api/user-post-events.md) |[event](event.md)| Erstellt ein neues Ereignis durch Veröffentlichen in der Instanzensammlung.|
|[Get event](../api/event-get.md) | [event](event.md) |Liest die Eigenschaften und Beziehungen eines Ereignisobjekts.|
|[Update](../api/event-update.md) | [event](event.md) |Aktualisiert das Ereignisobjekt. |
|[Delete](../api/event-delete.md) | Keine |Löscht das Ereignisobjekt. |
|[accept](../api/event-accept.md)|Keiner|Akzeptieren Sie das angegebene Ereignis in einem Benutzerkalender an.|
|[tentativelyAccept](../api/event-tentativelyaccept.md)|Keiner|Mit Vorbehalt annehmen Sie das angegebene Ereignis in einem Benutzerkalender ein.|
|[decline](../api/event-decline.md)|Keiner|Einladung auf das angegebene Ereignis in einem Benutzerkalender abzulehnen.|
|[delta](../api/event-delta.md)|[event](event.md)-Sammlung|Dient zum Abrufen einer Reihe von Ereignissen, die in einer **calendarView** (ein Bereich von Ereignissen) im primären Kalender des Benutzers hinzugefügt, gelöscht oder aktualisiert wurden.|
|[dismissReminder](../api/event-dismissreminder.md)|Keiner|Schließen Sie die Erinnerung für das angegebene Ereignis in einem Benutzerkalender an.|
|[snoozeReminder](../api/event-snoozereminder.md)|Keiner|Verschieben Sie eine Erinnerung für das angegebene Ereignis in einem Benutzerkalender bis zu einem neuen Zeitpunkt.|
|[List instances](../api/event-list-instances.md) |[Ereignissammlung](event.md)| Ruft alle Instanzen (Vorkommen) eines Ereignisses ab, die innerhalb eines angegebenen Zeitraums existieren. Wenn das Ereignis vom Typ `SeriesMaster` ist, werden hierdurch alle Vorkommen und Ausnahmen des Ereignisses zurückgegeben, die innerhalb des angegebenen Zeitraums existieren.|
|**Anlagen**| | |
|[List attachments](../api/event-list-attachments.md) |[attachment](attachment.md) collection| Ruft alle Anlagen für ein Ereignis ab.|
|[Hinzufügen einer Anlage](../api/event-post-attachments.md) |[attachment](attachment.md)| Fügt einem Ereignis eine neue Anlage durch Veröffentlichen in der Anlagensammlung hinzu.|
|**Offene Erweiterungen**| | |
|[Offene Erweiterung erstellen](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Erstellt eine offene Erweiterung und fügt benutzerdefinierte Eigenschaften in einer neuen oder vorhandenen Instanz einer Ressource hinzu.|
|[Offene Erweiterung abrufen](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md)-Sammlung| Ruft ein offenes Erweiterungsobjekt oder Objekte basierend auf ihrem Namen oder vollqualifizierten Namen ab.|
|**Erweiterte Eigenschaften**| | |
|[Create single-value extended property](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[event](event.md)  |Erstellt eine oder mehrere einwertige erweiterte Eigenschaften in einem neuen oder vorhandenen Ereignis.   |
|[Get event with single-value extended property](../api/singlevaluelegacyextendedproperty-get.md)  | [event](event.md) | Ruft mithilfe von `$expand` oder `$filter` Ereignisse mit einer bestimmten einwertigen erweiterten Eigenschaft ab. |
|[Create multi-value extended property](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [event](event.md) | Erstellt eine oder mehrere mehrwertige erweiterte Eigenschaften in einem neuen oder vorhandenen Ereignis.  |
|[Get event with multi-value extended property](../api/multivaluelegacyextendedproperty-get.md)  | [event](event.md) | Ruft mithilfe von `$expand` ein Ereignis mit einer bestimmten mehrwertigen erweiterten Eigenschaft ab. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|attendees|[attendee](attendee.md) collection|Die Sammlung der Teilnehmer des Ereignisses|
|body|[itemBody](itembody.md)|Der Text der Nachricht, die dem Ereignis zugeordnet ist. Er kann im HTML- oder Textformat vorliegen.|
|bodyPreview|Zeichenfolge|Die Vorschau der Nachricht, die dem Ereignis zugeordnet ist. Liegt im Textformat vor.|
|categories|String collection|Die Kategorien, die dem Ereignis zugeordnet sind|
|changeKey|Zeichenfolge|Gibt die Version des Ereignisobjekts an. Jedes Mal, wenn das Ereignis geändert wird, wird auch die Eigenschaft „changeKey“ geändert. Auf diese Weise kann Exchange Änderungen an der korrekten Version des Objekts vornehmen.|
|createdDateTime|DateTimeOffset|Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|end|[dateTimeTimeZone](datetimetimezone.md)|Datum, Uhrzeit und Zeitzone für das Ende des Ereignisses|
|hasAttachments|Boolean|„true“, wenn das Ereignis Anlagen hat|
|iCalUId|String|Ein eindeutiger Bezeichner, der für alle Instanzen eines Ereignisses in unterschiedlichen Kalendern verwendet wird Schreibgeschützt.|
|id|Zeichenfolge| Schreibgeschützt|
|importance|Wichtigkeit|Die Wichtigkeit des Ereignisses. Die möglichen Werte sind: `low`, `normal`, `high`.|
|isAllDay|Boolean|„true“, wenn das Ereignis ein ganztägiges Ereignis ist|
|isCancelled|Boolean|„true“, wenn das Ereignis abgesagt wurde|
|isOrganizer|Boolean|„true“, wenn der Absender der Nachricht auch der Organisator ist|
|isReminderOn|Boolean|„true“, wenn eingestellt ist, dass der Benutzer an das Ereignis erinnert werden soll|
|lastModifiedDateTime|DateTimeOffset|Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|location|[location](location.md)|Der Ort des Ereignisses.|
|locations|[location](location.md)-Sammlung|Die Orte, an denen die Veranstaltung stattfindet. Die Eigenschaften **location** und **locations** entsprechen sich immer gegenseitig. Wenn Sie die **location**-Eigenschaft aktualisieren, werden alle früheren Orte in der **locations**-Sammlung entfernt und durch den neuen **location**-Wert ersetzt. |
|onlineMeetingUrl|Zeichenfolge|Eine URL für eine Onlinebesprechung Die Eigenschaft wird nur beim Organisator ein Ereignisses, wie eine onlinebesprechung umwandeln, wie etwa einer Besprechung Skype angibt festgelegt. Schreibgeschützt.|
|organizer|[recipient](recipient.md)|Der Organisator des Ereignisses|
|originalEndTimeZone|String|Die Zeitzone, die bei der Erstellung des Ereignisses für das Ereignisende festgelegt wurde. Der Wert `tzone://Microsoft/Custom` gibt an, dass eine ältere benutzerdefinierte Zeitzone in Outlook Desktop festgelegt wurde.|
|originalStart|DateTimeOffset|Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|originalStartTimeZone|String|Die Zeitzone, die bei der Erstellung des Ereignisses für den Ereignisbeginn festgelegt wurde. Der Wert `tzone://Microsoft/Custom` gibt an, dass eine ältere benutzerdefinierte Zeitzone in Outlook Desktop festgelegt wurde. |
|recurrence|[patternedRecurrence](patternedrecurrence.md)|Das Serienmuster für das Ereignis.|
|reminderMinutesBeforeStart|Int32|Festlegung, wie viele Minuten vor Beginn des Ereignisses die Erinnerung angezeigt werden soll|
|responseRequested|Boolean|„true“, wenn der Absender eine Antwort erhalten soll, sobald das Ereignis angenommen oder abgelehnt wird|
|responseStatus|[responseStatus](responsestatus.md)|Typ der Antwort, die als Antwort auf eine Ereignisnachricht gesendet wurde|
|sensitivity|sensitivity| Die möglichen Werte sind: `normal`, `personal`, `private`, `confidential`.|
|seriesMasterId|String|Die ID für die Datenreihe master Terminserie, wenn dieses Ereignis Teil einer Serie ist.|
|showAs|freeBusyStatus|Der anzuzeigende Status. Die möglichen Werte sind: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.|
|start|[dateTimeTimeZone](datetimetimezone.md)|Datum, Uhrzeit und Zeitzone für den Beginn des Ereignisses|
|subject|Zeichenfolge|Der Text der Betreffzeile des Ereignisses|
|type|eventType|Der Ereignistyp. Die möglichen Werte sind: `singleInstance`, `occurrence`, `exception`, `seriesMaster`. Schreibgeschützt.|
|webLink|String|Die URL zum Öffnen des Ereignisses in Outlook Web App:<br/><br/>Das Ereignis wird im Browser geöffnet, wenn Sie über Outlook Web App bei Ihrem Postfach angemeldet sind. Sie werden aufgefordert, sich anzumelden, wenn Sie noch nicht beim Browser angemeldet sind.<br/><br/>Auf diese URL kann von einem iFrame aus zugegriffen werden.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|attachments|[attachment](attachment.md) collection|Die Sammlung der [FileAttachment](fileattachment.md)- und [ItemAttachment](itemattachment.md)-Anlagen des Ereignisses. Navigationseigenschaft. Schreibgeschützt Lässt Nullwerte zu.|
|Kalender|[Kalender](calendar.md)|Der Kalender, der das Ereignis enthält. Navigationseigenschaft. Schreibgeschützt|
|Erweiterungen|[Erweiterungssammlung](extension.md)|Die Sammlung der für das Ereignis definierten offenen Erweiterungen. Schreibgeschützt. Lässt Nullwerte zu.|
|instances|[Ereignissammlung](event.md)|Die Instanzen des Ereignisses. Navigationseigenschaft. Schreibgeschützt Lässt Nullwerte zu.|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Sammlung| Die Sammlung der für das Ereignis definierten mehrwertigen erweiterten Eigenschaften. Schreibgeschützt. Lässt Nullwerte zu.|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Sammlung| Die Sammlung der für das Ereignis definierten einwertigen erweiterten Eigenschaften. Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "attachments",
    "calendar",
    "extensions",
    "instances",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.outlookItem",
  "@odata.type": "microsoft.graph.event",
  "@odata.annotations": [
    {
      "property": "attachments",
      "capabilities": {
        "changeTracking": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "calendar",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "extensions",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "instances",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "attendees": [{"@odata.type": "microsoft.graph.attendee"}],
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "bodyPreview": "string",
  "categories": ["string"],
  "changeKey": "string",
  "createdDateTime": "String (timestamp)",
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "hasAttachments": true,
  "iCalUId": "string",
  "id": "string (identifier)",
  "importance": "String",
  "isAllDay": true,
  "isCancelled": true,
  "isOrganizer": true,
  "isReminderOn": true,
  "lastModifiedDateTime": "String (timestamp)",
  "location": {"@odata.type": "microsoft.graph.location"},
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "onlineMeetingUrl": "string",
  "organizer": {"@odata.type": "microsoft.graph.recipient"},
  "originalEndTimeZone": "string",
  "originalStart": "String (timestamp)",
  "originalStartTimeZone": "string",
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "reminderMinutesBeforeStart": 1024,
  "responseRequested": true,
  "responseStatus": {"@odata.type": "microsoft.graph.responseStatus"},
  "sensitivity": "String",
  "seriesMasterId": "string",
  "showAs": "String",
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "subject": "string",
  "type": "String",
  "webLink": "string",

  "attachments": [ { "@odata.type": "microsoft.graph.attachment" } ],
  "calendar": { "@odata.type": "microsoft.graph.calendar" },
  "extensions": [ { "@odata.type": "microsoft.graph.extension" } ],
  "instances": [ { "@odata.type": "microsoft.graph.event" }],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]

}

```


## <a name="see-also"></a>Siehe auch

- [Verwenden einer Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten](/graph/delta-query-overview)
- [Inkrementelle Änderungen an Ereignissen in einem Ordner abrufen](/graph/delta-query-events)
- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](/graph/extensibility-overview)
- [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen](/graph/extensibility-open-users)
- [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
