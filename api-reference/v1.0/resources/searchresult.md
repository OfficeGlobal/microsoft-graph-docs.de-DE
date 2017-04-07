# <a name="searchresult-resource-type"></a>SearchResult-Ressourcentyp

Die **SearchResult**-Ressource gibt an, dass ein Element die Antwort auf eine Suche ist.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "onClickTelemtryUrl" ],
  "@odata.type": "microsoft.graph.searchResult"
}-->

```json
{
  "onClickTelemetryUrl": "url"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft            | Typ   | Beschreibung                                                                                                                                                                         |
|:--------------------|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| onClickTelemetryUrl | String | Ein Rückruf-URL, die zum Erfassen von Telemetrieinformationen verwendet werden kann. Die Anwendung sollte ein GET für diese URL ausgeben, wenn der Benutzer mit diesem Element zur Verbesserung der Qualität der Ergebnisse interagiert. |

## <a name="remarks"></a>Bemerkungen 

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
