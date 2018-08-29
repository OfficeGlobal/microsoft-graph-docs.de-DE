# <a name="plannerappliedcategories-resource-type"></a>plannerAppliedCategories-Ressourcentyp


Die **AppliedCategoriesCollection**-Ressource stellt die Sammlung von Kategorien (oder Bezeichnungen) dar, die auf eine Aufgabe angewendet wurden. Sie ist Teil des [plannerTask](plannertask.md)-Objekts. Auf eine Aufgabe können bis zu 6 Kategorien angewendet werden. Kategoriebeschreibungen wie `category1`, `category2` usw. sind Teil des [planDetails ](plannerplandetails.md)-Objekts. Es handelt sich um einen offenen Typ.

## <a name="properties"></a>Eigenschaften
Eigenschaften mit offenem Typ können vom Client definiert werden. In diesem Fall muss der Client jedoch `category1`, `category2`, `category3`, `category4`, `category5` und/oder `category6` als Eigenschaften angeben, deren Wert das boolesche `true` ist, wenn die entsprechenden Kategorien auf die Aufgabe angewendet werden. Nachfolgend ein Beispiel. Wenn sie nicht zutreffen, werden Eigenschaften automatisch entfernt, indem ihre Werte auf das boolesche `false` festgelegt werden. 

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "String-value" ],
  "@odata.type": "microsoft.graph.plannerAppliedCategories"
}-->

```json
{
  "String-value": true
}
```

Beispiel: 

```json
{
  "category1": true,
  "category3": true,
  "category5": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAppliedCategories resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->