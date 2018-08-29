# <a name="attendee-resource-type"></a>attendee-Ressourcentyp

Ein Teilnehmer eines Ereignisses. Dies kann eine Person oder eine Ressource sein, wie z. B. Besprechungsräume oder Geräte, die als Ressource auf dem Exchange-Server für den Mandanten eingerichtet wurden.

Abgeleitet von [attendeeBase](attendeebase.md).

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|status|[ResponseStatus](responsestatus.md)|Die Antwort des Teilnehmers (keine, akzeptiert, abgelehnt, usw.) für das Ereignis und das Datum und die Uhrzeit, an dem/der die Antwort gesendet wurde.|
|Typ|String|Der Teilnehmertyp: `required`, `optional`, `resource`.|
|emailAddress|[emailAddress](emailaddress.md)|Enthält den Namen und die SMTP-Adresse des Teilnehmers.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attendeeBase",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendee"
}-->

```json
{
  "status": {"@odata.type": "microsoft.graph.responseStatus"},
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->