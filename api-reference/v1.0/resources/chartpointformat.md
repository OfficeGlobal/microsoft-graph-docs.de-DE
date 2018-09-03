# <a name="chartpointformat-resource-type"></a><span data-ttu-id="ebdff-101">ChartPointFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ebdff-101">ChartPointFormat resource type</span></span>

<span data-ttu-id="ebdff-102">Stellt das Formatierungsobjekt für Diagrammpunkte dar.</span><span class="sxs-lookup"><span data-stu-id="ebdff-102">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="ebdff-103">Methoden</span><span class="sxs-lookup"><span data-stu-id="ebdff-103">Methods</span></span>
<span data-ttu-id="ebdff-104">Keine</span><span class="sxs-lookup"><span data-stu-id="ebdff-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="ebdff-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ebdff-105">Properties</span></span>
<span data-ttu-id="ebdff-106">Keine</span><span class="sxs-lookup"><span data-stu-id="ebdff-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="ebdff-107">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ebdff-107">Relationships</span></span>
| <span data-ttu-id="ebdff-108">Beziehung</span><span class="sxs-lookup"><span data-stu-id="ebdff-108">Relationship</span></span> | <span data-ttu-id="ebdff-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ebdff-109">Type</span></span>   |<span data-ttu-id="ebdff-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ebdff-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ebdff-111">ausfüllen</span><span class="sxs-lookup"><span data-stu-id="ebdff-111">fill</span></span>|[<span data-ttu-id="ebdff-112">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="ebdff-112">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="ebdff-p101">Stellt das Füllungsformat eines Diagramms dar, einschließlich Informationen zur Hintergrundformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ebdff-p101">Represents the fill format of a chart, which includes background formating information. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="ebdff-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ebdff-115">JSON representation</span></span>

<span data-ttu-id="ebdff-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ebdff-116">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPointFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPointFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->