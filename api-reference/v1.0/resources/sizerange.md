# <a name="sizerange-resource-type"></a><span data-ttu-id="c8f65-101">sizeRange-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c8f65-101">sizeRange resource type</span></span>


<span data-ttu-id="c8f65-102">Gibt die maximale und minimale Größe (in Kilobyte) an, die eine eingehende Nachrichten aufweisen muss, damit eine Bedingung oder Ausnahme zutrifft.</span><span class="sxs-lookup"><span data-stu-id="c8f65-102">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="c8f65-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c8f65-103">Properties</span></span>
| <span data-ttu-id="c8f65-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c8f65-104">Property</span></span>     | <span data-ttu-id="c8f65-105">Typ</span><span class="sxs-lookup"><span data-stu-id="c8f65-105">Type</span></span>   |<span data-ttu-id="c8f65-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c8f65-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c8f65-107">maximumSize</span><span class="sxs-lookup"><span data-stu-id="c8f65-107">maximumSize</span></span> | <span data-ttu-id="c8f65-108">Int32</span><span class="sxs-lookup"><span data-stu-id="c8f65-108">Int32</span></span> | <span data-ttu-id="c8f65-109">Die maximale Größe (in Kilobyte), die eine eingehende Nachrichten aufweisen muss, damit eine Bedingung oder Ausnahme zutrifft.</span><span class="sxs-lookup"><span data-stu-id="c8f65-109">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="c8f65-110">minimumSize</span><span class="sxs-lookup"><span data-stu-id="c8f65-110">minimumSize</span></span> | <span data-ttu-id="c8f65-111">Int32</span><span class="sxs-lookup"><span data-stu-id="c8f65-111">Int32</span></span> | <span data-ttu-id="c8f65-112">Die minimale Größe (in Kilobyte), die eine eingehende Nachrichten aufweisen muss, damit eine Bedingung oder Ausnahme zutrifft.</span><span class="sxs-lookup"><span data-stu-id="c8f65-112">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="c8f65-113">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c8f65-113">JSON representation</span></span>
<span data-ttu-id="c8f65-114">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c8f65-114">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.sizeRange"
}-->

```json
{
  "maximumSize": "Int32",
  "minimumSize": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sizeRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->