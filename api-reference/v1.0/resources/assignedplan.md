# <a name="assignedplan-resource-type"></a><span data-ttu-id="ba3be-101">assignedPlan-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ba3be-101">assignedPlan resource type</span></span>

<span data-ttu-id="ba3be-102">Die **assignedPlans**-Eigenschaft der [user](user.md)-Entität und der [oganization](organization.md)-Entität ist eine Sammlung von **assignedPlan**.</span><span class="sxs-lookup"><span data-stu-id="ba3be-102">The **assignedPlans** property of both the [user](user.md) entity and the [organization](organization.md) entity is a collection of **assignedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="ba3be-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ba3be-103">Properties</span></span>
| <span data-ttu-id="ba3be-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ba3be-104">Property</span></span>     | <span data-ttu-id="ba3be-105">Typ</span><span class="sxs-lookup"><span data-stu-id="ba3be-105">Type</span></span>   |<span data-ttu-id="ba3be-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ba3be-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba3be-107">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba3be-107">assignedDateTime</span></span>|<span data-ttu-id="ba3be-108">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba3be-108">DateTimeOffset</span></span>|<span data-ttu-id="ba3be-p101">Datum und Uhrzeit der Zuweisung des Plans, z. B.: 2013-01-02T19:32:30Z. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ba3be-p101">The date and time at which the plan was assigned; for example: 2013-01-02T19:32:30Z. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ba3be-112">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="ba3be-112">capabilityStatus</span></span>|<span data-ttu-id="ba3be-113">String</span><span class="sxs-lookup"><span data-stu-id="ba3be-113">String</span></span>|<span data-ttu-id="ba3be-114">Z. B. „Aktiviert“.</span><span class="sxs-lookup"><span data-stu-id="ba3be-114">For example, “Enabled”.</span></span>|
|<span data-ttu-id="ba3be-115">service</span><span class="sxs-lookup"><span data-stu-id="ba3be-115">service</span></span>|<span data-ttu-id="ba3be-116">String</span><span class="sxs-lookup"><span data-stu-id="ba3be-116">String</span></span>|<span data-ttu-id="ba3be-117">Der Name des Diensts. z. B. „Exchange“.</span><span class="sxs-lookup"><span data-stu-id="ba3be-117">The name of the service; for example, “Exchange”.</span></span>|
|<span data-ttu-id="ba3be-118">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="ba3be-118">servicePlanId</span></span>|<span data-ttu-id="ba3be-119">Guid</span><span class="sxs-lookup"><span data-stu-id="ba3be-119">Guid</span></span>|<span data-ttu-id="ba3be-120">Eine GUID, die den Serviceplan identifiziert.</span><span class="sxs-lookup"><span data-stu-id="ba3be-120">A GUID that identifies the service plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ba3be-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ba3be-121">JSON representation</span></span>

<span data-ttu-id="ba3be-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ba3be-122">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedPlan"
}-->

```json
{
  "assignedDateTime": "String (timestamp)",
  "capabilityStatus": "string",
  "service": "string",
  "servicePlanId": "guid"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
