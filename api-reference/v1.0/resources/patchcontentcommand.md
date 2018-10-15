# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="f09a2-101">patchContentCommand-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f09a2-101">patchContentCommand resource type</span></span>

<span data-ttu-id="f09a2-102">Die an einer OneNote-Seite vorzunehmenden Änderungen in einer PATCH-Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f09a2-102">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f09a2-103">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f09a2-103">JSON representation</span></span>

<span data-ttu-id="f09a2-104">Es folgt eine JSON-Darstellung der Ressource, die im Text der Anforderung [PATCH pages/{id}\`](../api/page_update.md) gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="f09a2-104">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page_update.md) request.</span></span> 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenotePatchContentCommand"
}-->

```json
{
  "action": "String",
  "content": "string",
  "position": "String",
  "target": "string"
}

```

## <a name="properties"></a><span data-ttu-id="f09a2-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f09a2-105">Properties</span></span>
| <span data-ttu-id="f09a2-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f09a2-106">Property</span></span>     | <span data-ttu-id="f09a2-107">Typ</span><span class="sxs-lookup"><span data-stu-id="f09a2-107">Type</span></span>   |<span data-ttu-id="f09a2-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f09a2-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f09a2-109">Aktion</span><span class="sxs-lookup"><span data-stu-id="f09a2-109">action</span></span>|<span data-ttu-id="f09a2-110">onenotePatchActionType</span><span class="sxs-lookup"><span data-stu-id="f09a2-110">onenotePatchActionType values</span></span>|<span data-ttu-id="f09a2-111">Die auf das Zielelement anzuwendende Aktion.</span><span class="sxs-lookup"><span data-stu-id="f09a2-111">The action to perform on the target element.</span></span> <span data-ttu-id="f09a2-112">Die möglichen Werte sind: `replace`, `append`, `delete`, `insert`, oder`prepend`.</span><span class="sxs-lookup"><span data-stu-id="f09a2-112">The possible values are `replace`, `append`, `delete`, `insert`, , , , , , , , or `prepend`.</span></span>|
|<span data-ttu-id="f09a2-113">Inhalt</span><span class="sxs-lookup"><span data-stu-id="f09a2-113">content</span></span>|<span data-ttu-id="f09a2-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f09a2-114">String</span></span>|<span data-ttu-id="f09a2-p102">Eine Zeichenfolge aus wohlgeformtem HTML-Code, die der Seite hinzugefügt werden soll, sowie alle Bild- oder Dateibinärdaten. Wenn der Inhalt Binärdaten enthält, muss die Anforderung unter Verwendung des Inhaltstyps `multipart/form-data` mit der Komponente „Commands“ gesendet werden</span><span class="sxs-lookup"><span data-stu-id="f09a2-p102">A string of well-formed HTML to add to the page, and any image or file binary data. If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="f09a2-117">Position</span><span class="sxs-lookup"><span data-stu-id="f09a2-117">position</span></span>|<span data-ttu-id="f09a2-118">onenotePatchInsertPosition</span><span class="sxs-lookup"><span data-stu-id="f09a2-118">onenotePatchInsertPosition values</span></span>|<span data-ttu-id="f09a2-119">Die Position, an der der angegebene Inhalt hinzugefügt werden soll, relativ zum Zielelement.</span><span class="sxs-lookup"><span data-stu-id="f09a2-119">The location to add the supplied content, relative to the target element.</span></span> <span data-ttu-id="f09a2-120">Die möglichen Werte sind: `after` (Standard) oder `before`.</span><span class="sxs-lookup"><span data-stu-id="f09a2-120">The possible values are , , , , , , , , , , , or .</span></span>|
|<span data-ttu-id="f09a2-121">Ziel</span><span class="sxs-lookup"><span data-stu-id="f09a2-121">target</span></span>|<span data-ttu-id="f09a2-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f09a2-122">String</span></span>|<span data-ttu-id="f09a2-p104">Das zu aktualisierende Element. Muss die `#<data-id>` oder die generierte `<id>` des Elements oder das Schlüsselwort `body` oder `title` sein.</span><span class="sxs-lookup"><span data-stu-id="f09a2-p104">The element to update. Must be the `#<data-id>` or the generated `<id>` of the element, or the `body` or `title` keyword.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
