<span data-ttu-id="b9038-p102">Eigenschaften mit offenem Typ können vom Client definiert werden. In diesem Fall muss der Client jedoch `category1`, `category2`, `category3`, `category4`, `category5` und/oder `category6` als Eigenschaften angeben, deren Wert das boolesche `true` ist, wenn die entsprechenden Kategorien auf die Aufgabe angewendet werden. Nachfolgend ein Beispiel. Wenn sie nicht zutreffen, werden Eigenschaften automatisch entfernt, indem ihre Werte auf das boolesche `false` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="b9038-p102">Properties of an Open Type can be defined by the client. In this case though, the client must provide `category1`, `category2`, `category3`, `category4`, `category5` and/or `category6` as properties with their values being the `true` boolean when the corresponding categories are applied on the task. Example is shown below. When they do not apply, properties are automatically removed by setting their values to the `false` boolean.</span></span>
Eigenschaften mit offenem Typ können vom Client definiert werden. In diesem Fall muss der Client jedoch `category1`, `category2`, `category3`, `category4`, `category5` und/oder `category6` als Eigenschaften angeben, deren Wert das boolesche `true` ist, wenn die entsprechenden Kategorien auf die Aufgabe angewendet werden. Nachfolgend ein Beispiel. Wenn sie nicht zutreffen, werden Eigenschaften automatisch entfernt, indem ihre Werte auf das boolesche `false` festgelegt werden. 

## <span data-ttu-id="b9038-112">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b9038-112">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>

<span data-ttu-id="b9038-113">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b9038-113">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAppliedCategories"
}-->

```json
{
  "String-value": true
}
```

<span data-ttu-id="b9038-114">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="b9038-114">Example:</span></span> 

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