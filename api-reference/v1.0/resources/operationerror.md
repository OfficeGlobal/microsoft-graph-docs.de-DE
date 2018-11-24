# <a name="operationerror-resource-type"></a><span data-ttu-id="6e556-101">Ressourcentyp operationError</span><span class="sxs-lookup"><span data-stu-id="6e556-101">operationError resource type</span></span>



<span data-ttu-id="6e556-102">Fehler in [TeamsAsyncOperation](teamsasyncoperation.md)beschreibt.</span><span class="sxs-lookup"><span data-stu-id="6e556-102">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="6e556-103">OperationError Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6e556-103">operationError Properties</span></span>
| <span data-ttu-id="6e556-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6e556-104">Property</span></span>     | <span data-ttu-id="6e556-105">Typ</span><span class="sxs-lookup"><span data-stu-id="6e556-105">Type</span></span>   |<span data-ttu-id="6e556-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6e556-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e556-107">code</span><span class="sxs-lookup"><span data-stu-id="6e556-107">code</span></span>|<span data-ttu-id="6e556-108">Zeichenfolge (schreibgeschützt)</span><span class="sxs-lookup"><span data-stu-id="6e556-108">string (readonly)</span></span>|<span data-ttu-id="6e556-109">Fehlercode Vorgang.</span><span class="sxs-lookup"><span data-stu-id="6e556-109">Operation error code.</span></span>|
|<span data-ttu-id="6e556-110">message</span><span class="sxs-lookup"><span data-stu-id="6e556-110">message</span></span>|<span data-ttu-id="6e556-111">Zeichenfolge (schreibgeschützt)</span><span class="sxs-lookup"><span data-stu-id="6e556-111">string (readonly)</span></span>|<span data-ttu-id="6e556-112">Vorgang Fehlermeldung angezeigt.</span><span class="sxs-lookup"><span data-stu-id="6e556-112">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6e556-113">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6e556-113">JSON representation</span></span>

<span data-ttu-id="6e556-114">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6e556-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operationError"
}-->

```json
{
    "code": "TeamUnavailable",
    "message": "The team was not found."
}
```

<!-- uuid: 069fadaa-52db-4ced-85d5-74f7caa2c66f
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
