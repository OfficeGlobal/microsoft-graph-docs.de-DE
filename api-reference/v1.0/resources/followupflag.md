# <a name="followupflag-resource-type"></a>followupFlag-Ressourcentyp


Ermöglicht das Festlegen einer Kennzeichnung für den Benutzer zur späteren Weiterverfolgung. Unterstützte Elemente umfassen [message](message.md) und [contact](contact.md).

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|completedDateTime|[dateTimeTimeZone](dateTimeTimeZone.md)|Datum und Uhrzeit, zu dem bzw. der die Weiterverfolgung beendet wurde.|
|dueDateTime|**dateTimeTimeZone**|Datum und Uhrzeit, zu dem bzw. der die Weiterverfolgung beendet sein muss.|
|flagStatus|followupFlagStatus|Der Status für die Weiterverfolgung eines Elements. Mögliche Werte sind: `notFlagged`, `complete` und `flagged`.|
|startDateTime|**dateTimeTimeZone**|Datum und Uhrzeit, zu dem bzw. der die Weiterverfolgung beginnen soll.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.followupFlag"
}-->

```json
{
  "completedDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "dueDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "flagStatus": "String",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "followupFlag resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
