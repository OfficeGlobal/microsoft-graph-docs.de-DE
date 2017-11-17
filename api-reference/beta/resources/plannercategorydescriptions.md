# plannerCategoryDescriptions-Ressourcentyp
<a id="plannercategorydescriptions-resource-type" class="xliff"></a>

Die **plannerCategoryDescriptions**-Ressource stellt die beschreibenden Bezeichnungen für die Kategorien dar, die für einen Plan definiert wurden. Sie gehört zum [planDetails](plannerplandetails.md)-Objekt. Es können bis zu 6 Kategorien definiert werden. 


## Eigenschaften
<a id="properties" class="xliff"></a>
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|category1|String|Mit Kategorie 1 verknüpfte Bezeichnung.|
|category2|String|Mit Kategorie 2 verknüpfte Bezeichnung.|
|category3|String|Mit Kategorie 3 verknüpfte Bezeichnung.|
|category4|String|Mit Kategorie 4 verknüpfte Bezeichnung.|
|category5|String|Mit Kategorie 5 verknüpfte Bezeichnung.|
|category6|String|Mit Kategorie 6 verknüpfte Bezeichnung.|

## JSON-Darstellung
<a id="json-representation" class="xliff"></a>
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerCategoryDescriptions"
}-->

```json
{
  "category1": "String",
  "category2": "String",
  "category3": "String",
  "category4": "String",
  "category5": "String",
  "category6": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerCategoryDescriptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->