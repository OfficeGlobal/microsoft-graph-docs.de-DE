# <a name="serviceplaninfo-resource-type"></a><span data-ttu-id="8b6bf-101">servicePlanInfo-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8b6bf-101">servicePlanInfo resource type</span></span>

<span data-ttu-id="8b6bf-p101">Enthält Informationen zu einem Serviceplan, der einer abonnierten SKU zugeordnet ist. Die **servicePlans**-Eigenschaft der [subscribedSku](subscribedsku.md)-Entität ist eine Sammlung von **servicePlanInfo**.</span><span class="sxs-lookup"><span data-stu-id="8b6bf-p101">Contains information about a service plan associated with a subscribed SKU. The **servicePlans** property of the [subscribedSku](subscribedsku.md) entity is a collection of **servicePlanInfo**.</span></span>


## <a name="properties"></a><span data-ttu-id="8b6bf-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8b6bf-104">Properties</span></span>
| <span data-ttu-id="8b6bf-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8b6bf-105">Property</span></span>     | <span data-ttu-id="8b6bf-106">Typ</span><span class="sxs-lookup"><span data-stu-id="8b6bf-106">Type</span></span>   |<span data-ttu-id="8b6bf-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8b6bf-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b6bf-108">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="8b6bf-108">servicePlanId</span></span>|<span data-ttu-id="8b6bf-109">Guid</span><span class="sxs-lookup"><span data-stu-id="8b6bf-109">Guid</span></span>|<span data-ttu-id="8b6bf-110">Der eindeutige Bezeichner des Serviceplans.</span><span class="sxs-lookup"><span data-stu-id="8b6bf-110">The unique identifier of the service plan.</span></span>|
|<span data-ttu-id="8b6bf-111">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="8b6bf-111">servicePlanName</span></span>|<span data-ttu-id="8b6bf-112">String</span><span class="sxs-lookup"><span data-stu-id="8b6bf-112">String</span></span>|<span data-ttu-id="8b6bf-113">Der Name des Serviceplans.</span><span class="sxs-lookup"><span data-stu-id="8b6bf-113">The name of the service plan.</span></span>|
|<span data-ttu-id="8b6bf-114">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="8b6bf-114">provisioningStatus</span></span>|<span data-ttu-id="8b6bf-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8b6bf-115">String</span></span>|<span data-ttu-id="8b6bf-p102">Der Bereitstellungsstatus des Serviceplans. Mögliche Werte:</span><span class="sxs-lookup"><span data-stu-id="8b6bf-p102">The provisioning status of the service plan. Possible values:</span></span><br/><span data-ttu-id="8b6bf-118">„Success“ - Der Dienst wurde vollständig bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="8b6bf-118">"Success" - Service is fully provisioned.</span></span><br/><span data-ttu-id="8b6bf-119">„Disabled“ - Der Dienst wurde deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="8b6bf-119">"Disabled" - Service has been disabled.</span></span><br/><span data-ttu-id="8b6bf-120">„PendingInput“ - Der Dienst wurde noch nicht bereitgestellt, es wird auf die Dienstbestätigung gewartet.</span><span class="sxs-lookup"><span data-stu-id="8b6bf-120">"PendingInput" - Service is not yet provisioned; awaiting service confirmation.</span></span><br/><span data-ttu-id="8b6bf-121">„PendingActivation“ - Der Dienst wurde bereitgestellt, erfordert aber die explizite Aktivierung durch einen Administrator (z. B. Intune_O365-Serviceplan)</span><span class="sxs-lookup"><span data-stu-id="8b6bf-121">"PendingActivation" - Service is provisioned but requires explicit activation by administrator (for example, Intune_O365 service plan)</span></span><br/><span data-ttu-id="8b6bf-122">„PendingProvisioning“ - Microsoft hat einen neuen Dienst zur Produkt-SKU hinzugefügt, der noch nicht im Mandanten aktiviert wurde.</span><span class="sxs-lookup"><span data-stu-id="8b6bf-122">"PendingProvisioning" - Microsoft has added a new service to the product SKU and it has not been activated in the tenant, yet.</span></span>|
|<span data-ttu-id="8b6bf-123">appliesTo</span><span class="sxs-lookup"><span data-stu-id="8b6bf-123">appliesTo</span></span>|<span data-ttu-id="8b6bf-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8b6bf-124">String</span></span>|<span data-ttu-id="8b6bf-p103">Das Objekt, dem der Serviceplan zugewiesen werden kann. Mögliche Werte:</span><span class="sxs-lookup"><span data-stu-id="8b6bf-p103">The object the service plan can be assigned to. Possible values:</span></span><br/><span data-ttu-id="8b6bf-127">„User“ - Der Serviceplan kann einzelnen Benutzern zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="8b6bf-127">"User" - service plan can be assigned to individual users.</span></span><br/><span data-ttu-id="8b6bf-128">„Company“ - Der Serviceplan kann dem gesamten Mandanten zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="8b6bf-128">"Company" - service plan can be assigned to the entire tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8b6bf-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8b6bf-129">JSON representation</span></span>

<span data-ttu-id="8b6bf-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8b6bf-130">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.servicePlanInfo"
}-->

```json
{
  "appliesTo": "string",
  "provisioningStatus": "string",
  "servicePlanId": "guid",
  "servicePlanName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePlanInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
