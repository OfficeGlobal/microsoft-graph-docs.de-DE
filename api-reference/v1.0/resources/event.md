# <a name="event-resource-type"></a>Ressourcentyp „event“

Ein Ereignis in einem Kalender

Diese Ressource unterstützt Folgendes:

- Hinzufügen Ihrer eigenen Daten zu benutzerdefinierten Eigenschaften mithilfe von [Erweiterungen](../../../concepts/extensibility_overview.md).
- Verwenden einer [Delta-Abfrage](../../../concepts/delta_query_overview.md) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen der [delta](../api/event_delta.md)-Funktion.


## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[List events](../api/user_list_events.md)|[event](event.md) collection |Ruft eine Liste der [event](../resources/event.md)-Objekte im Postfach des Benutzers ab. Die Liste enthält einzelne Instanzen von Besprechungen und Serienmaster.|
|[Create event](../api/user_post_events.md) |[event](event.md)| Erstellt ein neues Ereignis durch Veröffentlichen in der Instanzensammlung.|
|[Get event](../api/event_get.md) | [event](event.md) |Liest die Eigenschaften und Beziehungen eines Ereignisobjekts.|
|[Update](../api/event_update.md) | [event](event.md) |Aktualisiert das Ereignisobjekt. |
|[Delete](../api/event_delete.md) | Keiner |Löscht das Ereignisobjekt. |
|[accept](../api/event_accept.md)|Keiner|Nimmt das angegebene Ereignis an.|
|[tentativelyAccept](../api/event_tentativelyaccept.md)|Keiner|Nimmt das angegebene Ereignis mit Vorbehalt an.|
|[decline](../api/event_decline.md)|Keiner|Lehnt die Einladung zu dem angegebenen Ereignis ab.|
|[delta](../api/event_delta.md)|[event](event.md)-Sammlung|Dient zum Abrufen einer Reihe von Ereignissen, die in einer **calendarView** (ein Bereich von Ereignissen) im primären Kalender des Benutzers hinzugefügt, gelöscht oder aktualisiert wurden.|
|[dismissReminder](../api/event_dismissreminder.md)|Keiner|Schließt die Erinnerung an das angegebene Ereignis.|
|[snoozeReminder](../api/event_snoozereminder.md)|Keiner|Legt fest, dass erneut an das Ereignis erinnert werden soll.|
|[List instances](../api/event_list_instances.md) |[Ereignissammlung](event.md)| Ruft alle Instanzen (Vorkommen) eines Ereignisses ab, die innerhalb eines angegebenen Zeitraums existieren. Wenn das Ereignis vom Typ `SeriesMaster` ist, werden hierdurch alle Vorkommen und Ausnahmen des Ereignisses zurückgegeben, die innerhalb des angegebenen Zeitraums existieren.|
|**Anlagen**| | |
|[List attachments](../api/event_list_attachments.md) |[attachment](attachment.md) collection| Ruft alle Anlagen für ein Ereignis ab.|
|[Hinzufügen einer Anlage](../api/event_post_attachments.md) |[attachment](attachment.md)| Fügt einem Ereignis eine neue Anlage durch Veröffentlichen in der Anlagensammlung hinzu.|
|**Offene Erweiterungen**| | |
|[Offene Erweiterung erstellen](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Erstellt eine offene Erweiterung und fügt benutzerdefinierte Eigenschaften in einer neuen oder vorhandenen Instanz einer Ressource hinzu.|
|[Offene Erweiterung abrufen](../api/opentypeextension_get.md) |[openTypeExtension](opentypeextension.md)-Sammlung| Ruft ein offenes Erweiterungsobjekt oder Objekte basierend auf ihrem Namen oder vollqualifizierten Namen ab.|
|**Erweiterte Eigenschaften**| | |
|[Create single-value extended property](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[event](event.md)  |Erstellt eine oder mehrere einwertige erweiterte Eigenschaften in einem neuen oder vorhandenen Ereignis.   |
|[Get event with single-value extended property](../api/singlevaluelegacyextendedproperty_get.md)  | [event](event.md) | Ruft mithilfe von `$expand` oder `$filter` Ereignisse mit einer bestimmten einwertigen erweiterten Eigenschaft ab. |
|[Create multi-value extended property](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [event](event.md) | Erstellt eine oder mehrere mehrwertige erweiterte Eigenschaften in einem neuen oder vorhandenen Ereignis.  |
|[Get event with multi-value extended property](../api/multivaluelegacyextendedproperty_get.md)  | [event](event.md) | Ruft mithilfe von `$expand` ein Ereignis mit einer bestimmten mehrwertigen erweiterten Eigenschaft ab. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|attendees|[attendee](attendee.md) collection|Die Sammlung der Teilnehmer des Ereignisses|
|body|[itemBody](itembody.md)|Der Text der Nachricht, die dem Ereignis zugeordnet ist. Er kann im HTML- oder Textformat vorliegen.|
|bodyPreview|String|Die Vorschau der Nachricht, die dem Ereignis zugeordnet ist. Liegt im Textformat vor.|
|categories|String collection|Die Kategorien, die dem Ereignis zugeordnet sind|
|changeKey|String|Gibt die Version des Ereignisobjekts an. Jedes Mal, wenn das Ereignis geändert wird, wird auch die Eigenschaft „changeKey“ geändert. Auf diese Weise kann Exchange Änderungen an der korrekten Version des Objekts vornehmen.|
|createdDateTime|DateTimeOffset|Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|end|[dateTimeTimeZone](datetimetimezone.md)|Datum, Uhrzeit und Zeitzone für das Ende des Ereignisses|
|hasAttachments|Boolean|„true“, wenn das Ereignis Anlagen hat|
|iCalUId|String|Ein eindeutiger Bezeichner, der für alle Instanzen eines Ereignisses in unterschiedlichen Kalendern verwendet wird|
|id|String| Schreibgeschützt|
|importance|String|Die Wichtigkeit des Ereignisses. Niedrig = 0, Normal = 1, Hoch = 2. Mögliche Werte: `Low`, `Normal`, `High`.|
|isAllDay|Boolean|„true“, wenn das Ereignis ein ganztägiges Ereignis ist|
|isCancelled|Boolean|„true“, wenn das Ereignis abgesagt wurde|
|isOrganizer|Boolean|„true“, wenn der Absender der Nachricht auch der Organisator ist|
|isReminderOn|Boolean|„true“, wenn eingestellt ist, dass der Benutzer an das Ereignis erinnert werden soll|
|lastModifiedDateTime|DateTimeOffset|Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|location|[location](location.md)|Der Ort, an dem das Ereignis stattfindet|
|onlineMeetingUrl|String|Eine URL für eine Onlinebesprechung|
|organizer|[recipient](recipient.md)|Der Organisator des Ereignisses|
|originalEndTimeZone|String|Die Zeitzone, die bei der Erstellung des Ereignisses für das Ereignisende festgelegt wurde. Der Wert `tzone://Microsoft/Custom` gibt an, dass eine ältere benutzerdefinierte Zeitzone in Outlook Desktop festgelegt wurde.|
|originalStart|DateTimeOffset|Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|originalStartTimeZone|String|Die Zeitzone, die bei der Erstellung des Ereignisses für den Ereignisbeginn festgelegt wurde. Der Wert `tzone://Microsoft/Custom` gibt an, dass eine ältere benutzerdefinierte Zeitzone in Outlook Desktop festgelegt wurde. |
|recurrence|[patternedRecurrence](patternedrecurrence.md)|Das Serienmuster für das Ereignis.|
|reminderMinutesBeforeStart|Int32|Festlegung, wie viele Minuten vor Beginn des Ereignisses die Erinnerung angezeigt werden soll|
|responseRequested|Boolean|„true“, wenn der Absender eine Antwort erhalten soll, sobald das Ereignis angenommen oder abgelehnt wird|
|responseStatus|[responseStatus](responsestatus.md)|Typ der Antwort, die als Antwort auf eine Ereignisnachricht gesendet wurde|
|sensitivity|String| Mögliche Werte: `Normal`, `Personal`, `Private`, `Confidential`|
|seriesMasterId|String|Die dem Element zugeordneten Kategorien|
|showAs|String|Der anzuzeigende Status: Frei = 0, Mit Vorbehalt = 1, Beschäftigt = 2, Abwesend = 3, An anderem Ort tätig = 4; Unbekannt =-1. Mögliche Werte: `Free`, `Tentative`, `Busy`, `Oof`, `WorkingElsewhere`, `Unknown`.|
|start|[dateTimeTimeZone](datetimetimezone.md)|Datum, Uhrzeit und Zeitzone für den Beginn des Ereignisses|
|subject|String|Der Text der Betreffzeile des Ereignisses|
|type|String|Der Ereignistyp: SingleInstance = 0, Occurrence = 1, Exception = 2, SeriesMaster = 3. Mögliche Werte: `SingleInstance`, `Occurrence`, `Exception`, `SeriesMaster`.|
|webLink|String|Die URL zum Öffnen des Ereignisses in Outlook Web App:<br/><br/>Das Ereignis wird im Browser geöffnet, wenn Sie über Outlook Web App bei Ihrem Postfach angemeldet sind. Sie werden aufgefordert, sich anzumelden, wenn Sie noch nicht beim Browser angemeldet sind.<br/><br/>Auf diese URL kann von einem iFrame aus zugegriffen werden.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|attachments|[attachment](attachment.md) collection|Die Sammlung der [FileAttachment](fileAttachment.md)- und [ItemAttachment](itemAttachment.md)-Anlagen des Ereignisses. Navigationseigenschaft. Schreibgeschützt. Lässt Nullwerte zu.|
|calendar|[calendar](calendar.md)|Der Kalender, der das Ereignis enthält. Navigationseigenschaft. Schreibgeschützt.|
|Erweiterungen|[Erweiterungssammlung](extension.md)|Die Sammlung der für das Ereignis definierten offenen Erweiterungen. Schreibgeschützt. Lässt Nullwerte zu.|
|instances|[event](event.md) collection|Die Instanzen des Ereignisses. Navigationseigenschaft. Schreibgeschützt. Lässt NULL-Werte zu.|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection| Die Sammlung der für das Ereignis definierten mehrwertigen erweiterten Eigenschaften. Schreibgeschützt. Lässt NULL-Werte zu.|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| Die Sammlung der für das Ereignis definierten einwertigen erweiterten Eigenschaften. Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "calendar",
    "extensions",
    "instances",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.event"
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

- [Verwenden einer Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten](../../../concepts/delta_query_overview.md)
- [Inkrementelle Änderungen an Ereignissen in einem Ordner abrufen](../../../concepts/delta_query_events.md)
- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](../../../concepts/extensibility_overview.md)
- [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen](../../../concepts/extensibility_open_users.md)
- [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
