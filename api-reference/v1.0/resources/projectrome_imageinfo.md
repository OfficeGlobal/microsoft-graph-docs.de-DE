# <a name="imageinfo-resource-type"></a>imageInfo Ressourcentyp

Ein komplexer Typ für die Eigenschaft **Zuweisung** im Teil [visualInfo](../resources/projectrome_visualinfo.md) des Objekts [Aktivität](../resources/projectrome_activity.md).

## <a name="properties"></a>Eigenschaften

|Name | Typ | Beschreibung|
|:----|:-----|:-----------|
|iconUrl | String | Optional; URI, der auf ein Symbol verweist, das die Anwendung verwendet, um die Aktivität zu generieren|
|alternateText | String | Optional; alternativer Text-Inhalt für das Bild|
|addImageQuery | Boolean | Optional; Parameter, um anzuzeigen, dass der Server als Reaktion auf Parametrisierung das Bild dynamisch rendern kann. Zum Beispiel – ein Bild mit hohem Kontrast|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "iconUrl",
    "alternateText",
    "addImageQuery"
  ],
  "@odata.type": "microsoft.graph.imageInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.imageInfo",
    "iconUrl": "String (URL)",
    "alternateText": "String",
    "addImageQuery": "boolean"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->