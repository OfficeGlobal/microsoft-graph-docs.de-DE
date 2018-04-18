# <a name="timezoneinformation-resource-type"></a>timeZoneInformation-Ressourcentyp


Stellt eine Zeitzone dar. Das unterstützte Format ist Windows und auch das Format der [IANA-Zeitzone (Internet Assigned Numbers Authority)](http://www.iana.org/time-zones) (auch bekannt als Olson-Zeitzone) wenn das derzeitige bekannte Problem behoben ist.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Alias|Zeichenfolge|Ein Bezeichner für die Zeitzone.|
|displayName|Zeichenfolge|Eine Anzeigezeichenfolge, die die Zeitzone darstellt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneInformation"
}-->

```json
{
  "alias": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeZoneInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->