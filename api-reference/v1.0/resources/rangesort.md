# <a name="rangesort-resource-type"></a><span data-ttu-id="a70e5-101">RangeSort-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a70e5-101">RangeSort resource type</span></span>

<span data-ttu-id="a70e5-102">Verwaltet Sortiervorgänge für Range-Objekte.</span><span class="sxs-lookup"><span data-stu-id="a70e5-102">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="a70e5-103">Methoden</span><span class="sxs-lookup"><span data-stu-id="a70e5-103">Methods</span></span>

| <span data-ttu-id="a70e5-104">Methode</span><span class="sxs-lookup"><span data-stu-id="a70e5-104">Method</span></span>           | <span data-ttu-id="a70e5-105">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="a70e5-105">Return Type</span></span>    |<span data-ttu-id="a70e5-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a70e5-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a70e5-107">Anwenden</span><span class="sxs-lookup"><span data-stu-id="a70e5-107">Apply</span></span>](../api/rangesort_apply.md)|<span data-ttu-id="a70e5-108">Keine</span><span class="sxs-lookup"><span data-stu-id="a70e5-108">None</span></span>|<span data-ttu-id="a70e5-109">Führt einen Sortiervorgang aus.</span><span class="sxs-lookup"><span data-stu-id="a70e5-109">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="a70e5-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a70e5-110">Properties</span></span>
<span data-ttu-id="a70e5-111">Keine</span><span class="sxs-lookup"><span data-stu-id="a70e5-111">None</span></span>

## <a name="relationships"></a><span data-ttu-id="a70e5-112">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a70e5-112">Relationships</span></span>
<span data-ttu-id="a70e5-113">Keine</span><span class="sxs-lookup"><span data-stu-id="a70e5-113">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a70e5-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a70e5-114">JSON representation</span></span>

<span data-ttu-id="a70e5-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a70e5-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookRangeSort"
}-->

```json
{
}
```

##### <a name="request"></a><span data-ttu-id="a70e5-116">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a70e5-116">Request</span></span>
<span data-ttu-id="a70e5-117">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a70e5-117">Here is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```

##### <a name="response"></a><span data-ttu-id="a70e5-118">Antwort</span><span class="sxs-lookup"><span data-stu-id="a70e5-118">Response</span></span>
<span data-ttu-id="a70e5-119">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a70e5-119">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeSort"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->