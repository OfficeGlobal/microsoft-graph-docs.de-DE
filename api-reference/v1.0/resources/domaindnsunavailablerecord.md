# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="f0129-101">domainDnsUnavailableRecord-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f0129-101">domainDnsUnavailableRecord resource type</span></span>

<span data-ttu-id="f0129-p101">Wenn Sie die Navigationseigenschaft **serviceConfigurationRecords** für eine [Domain](domain.md)-Entität abfragen, werden möglicherweise eine oder mehrere [DomainDnsCnameRecord](domaindnscnamerecord.md)-, [DomainDnsMxRecord](domaindnsmxrecord.md)-, [DomainDnsSrvRecord](domaindnssrvrecord.md)- und/oder [DomainDnsTxtRecord](domaindnstxtrecord.md)-Entitäten zurückgegeben. Diese Entitäten geben die DNS-Einträge an, die Sie der Zonendatei der Domäne hinzufügen müssen, bevor die Domäne von Microsoft-Onlinediensten verwendet werden kann. Wenn es nicht möglich ist, solche Entitäten zu generieren, wird stattdessen eine DomainDnsUnavailableRecord-Entität zurückgegeben. Geerbt von der Entität [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="f0129-p101">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities. These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services. When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="f0129-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="f0129-106">Methods</span></span>
<span data-ttu-id="f0129-p102">Direkte Abfragen dieser Ressource werden nicht unterstützt. Informationen zum Abfragen von Domänendiensteinträgen finden Sie im Thema [Domäne](domain.md).</span><span class="sxs-lookup"><span data-stu-id="f0129-p102">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="f0129-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f0129-109">Properties</span></span>
| <span data-ttu-id="f0129-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f0129-110">Property</span></span>     | <span data-ttu-id="f0129-111">Typ</span><span class="sxs-lookup"><span data-stu-id="f0129-111">Type</span></span>   |<span data-ttu-id="f0129-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f0129-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0129-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f0129-113">description</span></span>|<span data-ttu-id="f0129-114">String</span><span class="sxs-lookup"><span data-stu-id="f0129-114">String</span></span>|<span data-ttu-id="f0129-115">Gibt den Grund an, warum die **DomainDnsUnavailableRecord**-Entität zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="f0129-115">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f0129-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f0129-116">Relationships</span></span>
<span data-ttu-id="f0129-117">Keine</span><span class="sxs-lookup"><span data-stu-id="f0129-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0129-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f0129-118">JSON representation</span></span>
<span data-ttu-id="f0129-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f0129-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsUnavailableRecord"
}-->

```json
{
  "description": "String"
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