# <a name="educationorganization-resource-type"></a>Ressourcentyp educationOrganization

Abstrakte Entität zum Modellieren der Gemeinsamkeit zwischen verschiedenen Organisationstypen im Bildungsbereichs.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Beschreibung|Zeichenfolge| Beschreibung der Organisation.|
|displayName|Zeichenfolge| Anzeigename der Organisation.|
|externalSource|educationExternalSource| Die Quelle, aus der diese Organisation erstellt wurde. Mögliche Werte sind: `sis`, `manual` und `unknownFutureValue`.|

## <a name="relationships"></a>Beziehungen
Keine.


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOrganization"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "externalSource": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->