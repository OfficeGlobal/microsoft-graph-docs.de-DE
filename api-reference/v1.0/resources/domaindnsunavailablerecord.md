<span data-ttu-id="7353c-p102">Direkte Abfragen dieser Ressource werden nicht unterstützt. Informationen zum Abfragen von Domänendiensteinträgen finden Sie im Thema [Domäne](domain.md).</span><span class="sxs-lookup"><span data-stu-id="7353c-p102">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>
Direkte Abfragen dieser Ressource werden nicht unterstützt. Informationen zum Abfragen von Domänendiensteinträgen finden Sie im Thema [Domäne](domain.md).

## <span data-ttu-id="7353c-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7353c-109">Properties</span></span>
<a id="properties" class="xliff"></a>
| <span data-ttu-id="7353c-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7353c-110">Property</span></span>     | <span data-ttu-id="7353c-111">Typ</span><span class="sxs-lookup"><span data-stu-id="7353c-111">Type</span></span>   |<span data-ttu-id="7353c-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7353c-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7353c-113">description</span><span class="sxs-lookup"><span data-stu-id="7353c-113">description</span></span>|<span data-ttu-id="7353c-114">String</span><span class="sxs-lookup"><span data-stu-id="7353c-114">String</span></span>|<span data-ttu-id="7353c-115">Gibt den Grund an, warum die **DomainDnsUnavailableRecord**-Entität zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="7353c-115">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <span data-ttu-id="7353c-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7353c-116">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="7353c-117">Keine</span><span class="sxs-lookup"><span data-stu-id="7353c-117">None</span></span>

## <span data-ttu-id="7353c-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7353c-118">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="7353c-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7353c-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsUnavailableRecord"
}-->

```json
{
  "canonicalName": "String",
  "description": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "text": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsUnavailableRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->