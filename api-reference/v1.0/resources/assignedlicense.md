# <a name="assignedlicense-resource-type"></a><span data-ttu-id="bd38e-101">assignedLicense-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bd38e-101">assignedLicense resource type</span></span>

<span data-ttu-id="bd38e-p101">Stellt eine Lizenz dar, die einem Benutzer zugewiesen ist. Die **assignedLicenses**-Eigenschaft der [user](user.md)-Entität ist eine Sammlung von **assignedLicense**.</span><span class="sxs-lookup"><span data-stu-id="bd38e-p101">Represents a license assigned to a user. The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="bd38e-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bd38e-104">Properties</span></span>
| <span data-ttu-id="bd38e-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bd38e-105">Property</span></span>     | <span data-ttu-id="bd38e-106">Typ</span><span class="sxs-lookup"><span data-stu-id="bd38e-106">Type</span></span>   |<span data-ttu-id="bd38e-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bd38e-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd38e-108">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="bd38e-108">disabledPlans</span></span>|<span data-ttu-id="bd38e-109">GUID-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bd38e-109">Guid collection</span></span>|<span data-ttu-id="bd38e-110">Eine Auflistung der eindeutigen Bezeichner für Pläne, die deaktiviert wurden.</span><span class="sxs-lookup"><span data-stu-id="bd38e-110">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="bd38e-111">skuId</span><span class="sxs-lookup"><span data-stu-id="bd38e-111">skuId</span></span>|<span data-ttu-id="bd38e-112">Guid</span><span class="sxs-lookup"><span data-stu-id="bd38e-112">Guid</span></span>|<span data-ttu-id="bd38e-113">Die eindeutige ID der SKU.</span><span class="sxs-lookup"><span data-stu-id="bd38e-113">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bd38e-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bd38e-114">JSON representation</span></span>

<span data-ttu-id="bd38e-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bd38e-115">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedLicense"
}-->

```json
{
  "disabledPlans": ["guid"],
  "skuId": "guid"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignedLicense resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
