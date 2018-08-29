# <a name="provisionedplan-resource-type"></a><span data-ttu-id="eb1e5-101">provisionedPlan-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="eb1e5-101">provisionedPlan resource type</span></span>

<span data-ttu-id="eb1e5-102">Die **ProvisionedPlans**-Eigenschaft der [user](user.md)-Entität und der [oganization](organization.md)-Entität ist eine Sammlung von **provisionedPlan**.</span><span class="sxs-lookup"><span data-stu-id="eb1e5-102">The **provisionedPlans** property of the [user](user.md) entity and the [organization](organization.md) entity is a collection of **provisionedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="eb1e5-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="eb1e5-103">Properties</span></span>
| <span data-ttu-id="eb1e5-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eb1e5-104">Property</span></span>     | <span data-ttu-id="eb1e5-105">Typ</span><span class="sxs-lookup"><span data-stu-id="eb1e5-105">Type</span></span>   |<span data-ttu-id="eb1e5-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eb1e5-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb1e5-107">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="eb1e5-107">capabilityStatus</span></span>|<span data-ttu-id="eb1e5-108">String</span><span class="sxs-lookup"><span data-stu-id="eb1e5-108">String</span></span>|<span data-ttu-id="eb1e5-109">Z. B. „Aktiviert“.</span><span class="sxs-lookup"><span data-stu-id="eb1e5-109">For example, “Enabled”.</span></span>|
|<span data-ttu-id="eb1e5-110">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="eb1e5-110">provisioningStatus</span></span>|<span data-ttu-id="eb1e5-111">String</span><span class="sxs-lookup"><span data-stu-id="eb1e5-111">String</span></span>|<span data-ttu-id="eb1e5-112">Z. B. „Erfolgreich“.</span><span class="sxs-lookup"><span data-stu-id="eb1e5-112">For example, “Success”.</span></span>|
|<span data-ttu-id="eb1e5-113">service</span><span class="sxs-lookup"><span data-stu-id="eb1e5-113">service</span></span>|<span data-ttu-id="eb1e5-114">String</span><span class="sxs-lookup"><span data-stu-id="eb1e5-114">String</span></span>|<span data-ttu-id="eb1e5-115">Der Name des Diensts. z. B. „AccessControlS2S“</span><span class="sxs-lookup"><span data-stu-id="eb1e5-115">The name of the service; for example, “AccessControlS2S”</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eb1e5-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="eb1e5-116">JSON representation</span></span>

<span data-ttu-id="eb1e5-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="eb1e5-117">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedPlan"
}-->

```json
{
  "capabilityStatus": "string",
  "provisioningStatus": "string",
  "service": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisionedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->