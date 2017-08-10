# <a name="settingvalue-resource-type"></a>settingValue-Ressourcentyp

Eine Einstellung, die durch ein Name/Wertpaar dargestellt wird.

### <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------------|:--------|:----------|
|name|Zeichenfolge| Name der Einstellung (entsprechend der [groupSettingTemplate](groupsettingtemplate.md)-Definition). |
|Wert|Zeichenfolge| Wert der Einstellung. |

### <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingValue"
}-->

```json
{
  "name": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->