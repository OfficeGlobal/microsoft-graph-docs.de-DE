# <a name="educationterm-resource-type"></a>educationTerm-Ressourcentyp

Ein Zeitraum. Er stellt einen festgelegten Teil des akademischen Jahres dar. Er wird in [educationClass](educationclass.md) verwendet.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|displayName| String| Der Anzeigename des Zeitraums| 
|externalId|String| Die ID des Zeitraums im Synchronisierungssystem|
|startDate|Date|Anfang des Zeitraums|
|endDate|Date|Ende des Zeitraums|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTerm"
}-->

```json
{
  "displayName": "String",
  "externalId": "String",
  "startDate": "Date",
  "endDate": "Date"
}
```

<!-- uuid: 4e9d671f-3068-4e09-aba2-b39e81a0e452
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationTerm resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->