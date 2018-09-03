# <a name="automaticrepliesmailtips-resource-type"></a>Ressourcentyp automaticRepliesMailTips


[E-Mail-Infos](../resources/mailtips.md) zu automatischen Antworten, die für ein Postfach eingerichtet wurden.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:-----|:-----|:-----|
| Nachricht | Zeichenfolge | Die Nachricht der automatischen Antwort. |
| messageLanguage | [localeInfo](../resources/localeinfo.md) | Die Sprache der Nachricht der automatischen Antwort. |
| scheduledEndTime | [dateTimeTimeZone](../resources/datetimetimezone.md) | Das Datum und die Uhrzeit, für die das Ende der automatischen Antworten festgelegt wurde. |
| scheduledStartTime | [dateTimeTimeZone](../resources/datetimetimezone.md) | Datum und Uhrzeit, für die der Beginn der automatischen Antworten festgelegt wurde. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messageLanguage",
    "scheduledEndTime",
    "scheduledStartTime"
  ],
  "@odata.type": "microsoft.graph.automaticRepliesMailTips"
}-->

```json
{
  "message": "string",
  "messageLanguage": {"@odata.type": "microsoft.graph.localeInfo"},
  "scheduledEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesMailTips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->