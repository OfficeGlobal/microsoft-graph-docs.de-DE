# <a name="verifieddomain-resource-type"></a><span data-ttu-id="45cb9-101">verifiedDomain-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="45cb9-101">verifiedDomain resource type</span></span>

<span data-ttu-id="45cb9-p101">Gibt eine Domäne für einen Mandanten an. Die **verifiedDomains**-Eigenschaft der [organization](organization.md)-Entität ist eine Auflistung von **VerifiedDomain**.</span><span class="sxs-lookup"><span data-stu-id="45cb9-p101">Specifies a domain for a tenant. The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="45cb9-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="45cb9-104">Properties</span></span>
| <span data-ttu-id="45cb9-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="45cb9-105">Property</span></span>     | <span data-ttu-id="45cb9-106">Typ</span><span class="sxs-lookup"><span data-stu-id="45cb9-106">Type</span></span>   |<span data-ttu-id="45cb9-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="45cb9-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="45cb9-108">Funktionen</span><span class="sxs-lookup"><span data-stu-id="45cb9-108">capabilities</span></span>|<span data-ttu-id="45cb9-109">String</span><span class="sxs-lookup"><span data-stu-id="45cb9-109">String</span></span>|<span data-ttu-id="45cb9-110">Zum Beispiel „Email“, „OfficeCommunicationsOnline“.</span><span class="sxs-lookup"><span data-stu-id="45cb9-110">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="45cb9-111">isDefault</span><span class="sxs-lookup"><span data-stu-id="45cb9-111">isDefault</span></span>|<span data-ttu-id="45cb9-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="45cb9-112">Boolean</span></span>|                <span data-ttu-id="45cb9-113">**true**, wenn dies die Standarddomäne ist, die dem Mandanten zugeordnet ist, andernfalls **false**.</span><span class="sxs-lookup"><span data-stu-id="45cb9-113">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="45cb9-114">isInitial</span><span class="sxs-lookup"><span data-stu-id="45cb9-114">isInitial</span></span>|<span data-ttu-id="45cb9-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="45cb9-115">Boolean</span></span>|<span data-ttu-id="45cb9-116">**true**, wenn dies die ursprüngliche Domäne ist, die dem Mandanten zugeordnet ist, andernfalls **false**.</span><span class="sxs-lookup"><span data-stu-id="45cb9-116">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="45cb9-117">name</span><span class="sxs-lookup"><span data-stu-id="45cb9-117">name</span></span>|<span data-ttu-id="45cb9-118">String</span><span class="sxs-lookup"><span data-stu-id="45cb9-118">String</span></span>|<span data-ttu-id="45cb9-119">Der Domänenname, zum Beispiel „contoso.onmicrosoft.com“</span><span class="sxs-lookup"><span data-stu-id="45cb9-119">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="45cb9-120">type</span><span class="sxs-lookup"><span data-stu-id="45cb9-120">type</span></span>|<span data-ttu-id="45cb9-121">String</span><span class="sxs-lookup"><span data-stu-id="45cb9-121">String</span></span>|<span data-ttu-id="45cb9-122">Z. B. „verwaltet“.</span><span class="sxs-lookup"><span data-stu-id="45cb9-122">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="45cb9-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="45cb9-123">JSON representation</span></span>

<span data-ttu-id="45cb9-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="45cb9-124">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifieddomain"
}-->

```json
{
  "capabilities": "string",
  "isDefault": true,
  "isInitial": true,
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "verifiedDomain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
