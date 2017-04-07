# <a name="alternativesecurityid-resource-type"></a>alternativeSecurityId-Ressourcentyp

Enthält eine alternative Sicherheits-ID, die mit einem Gerät verknüpft ist. Die **alternativeSecurityIds**-Eigenschaft der [Device](device.md)-Entität ist eine Sammlung von **alternativeSecurityId**.

## <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|identityProvider|String|            |
|Key|Binär|            |
|Typ|Int32|            |


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.alternativeSecurityId"
}-->

```json
{
  "identityProvider": "string",
  "key": "binary",
  "type": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alternativeSecurityId resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
