# <a name="operation-resource-type"></a><span data-ttu-id="de980-101">Vorgangs-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="de980-101">operation resource type</span></span>

<span data-ttu-id="de980-102">Der Status eines zeitintensiven Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="de980-102">The status of a long-running operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="de980-103">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="de980-103">JSON representation</span></span>

<span data-ttu-id="de980-104">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="de980-104">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.operation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "lastActionDateTime": "String (timestamp)",
  "status": "notStarted | running | completed | failed"
}

```
## <a name="properties"></a><span data-ttu-id="de980-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="de980-105">Properties</span></span>
| <span data-ttu-id="de980-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="de980-106">Property</span></span>     | <span data-ttu-id="de980-107">Typ</span><span class="sxs-lookup"><span data-stu-id="de980-107">Type</span></span>   |<span data-ttu-id="de980-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="de980-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de980-109">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="de980-109">createdDateTime</span></span>| <span data-ttu-id="de980-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de980-110">DateTimeOffset</span></span> |<span data-ttu-id="de980-111">Die Startzeit des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="de980-111">The start time of the operation.</span></span>|
|<span data-ttu-id="de980-112">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="de980-112">lastActionDateTime</span></span>| <span data-ttu-id="de980-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de980-113">DateTimeOffset</span></span> |<span data-ttu-id="de980-114">Der Zeitpunkt der letzten Aktion des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="de980-114">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="de980-115">Status</span><span class="sxs-lookup"><span data-stu-id="de980-115">status</span></span>|<span data-ttu-id="de980-116">operationStatus</span><span class="sxs-lookup"><span data-stu-id="de980-116">operationStatus</span></span>|<span data-ttu-id="de980-117">Der aktuellen Status des Vorgangs: `notStarted`, `running`, `completed`, `failed`</span><span class="sxs-lookup"><span data-stu-id="de980-117">The current status of the operation: `notStarted`, `running`, `completed`, `failed`</span></span> |

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
