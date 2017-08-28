# <a name="itembody-resource-type"></a><span data-ttu-id="b9a64-101">itemBody-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b9a64-101">itemBody resource type</span></span>

<span data-ttu-id="b9a64-102">Stellt Eigenschaften des Textkörpers eines Elements dar, z. B. eine Nachricht, ein Ereignis oder ein Gruppenbeitrag.</span><span class="sxs-lookup"><span data-stu-id="b9a64-102">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="b9a64-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b9a64-103">Properties</span></span>
| <span data-ttu-id="b9a64-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b9a64-104">Property</span></span>     | <span data-ttu-id="b9a64-105">Typ</span><span class="sxs-lookup"><span data-stu-id="b9a64-105">Type</span></span>   |<span data-ttu-id="b9a64-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9a64-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9a64-107">Inhalt</span><span class="sxs-lookup"><span data-stu-id="b9a64-107">content</span></span>|<span data-ttu-id="b9a64-108">String</span><span class="sxs-lookup"><span data-stu-id="b9a64-108">String</span></span>|<span data-ttu-id="b9a64-109">Der Inhalt des Elements.</span><span class="sxs-lookup"><span data-stu-id="b9a64-109">The content of the item.</span></span>|
|<span data-ttu-id="b9a64-110">contentType</span><span class="sxs-lookup"><span data-stu-id="b9a64-110">contentType</span></span>|<span data-ttu-id="b9a64-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b9a64-111">String</span></span>|<span data-ttu-id="b9a64-p101">Der Typ des Inhalts. Mögliche Werte sind `Text` und `HTML`.</span><span class="sxs-lookup"><span data-stu-id="b9a64-p101">The type of the content. Possible values are `Text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b9a64-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b9a64-114">JSON representation</span></span>

<span data-ttu-id="b9a64-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b9a64-115">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemBody"
}-->

```json
{
  "content": "string",
  "contentType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemBody resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
