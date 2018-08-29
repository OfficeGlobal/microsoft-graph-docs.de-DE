# <a name="domaindnstxtrecord-resource-type"></a><span data-ttu-id="c3bda-101">domainDnsTxtRecord-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c3bda-101">domainDnsTxtRecord resource type</span></span>

<span data-ttu-id="c3bda-p101">Stellt einen TXT-Eintrag dar, der der DNS-Zonendatei einer bestimmten Domäne im Mandanten hinzugefügt wird. Geerbt von der Entität [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="c3bda-p101">Represents a TXT record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="c3bda-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="c3bda-104">Methods</span></span>
<span data-ttu-id="c3bda-p102">Direkte Abfragen dieser Ressource werden nicht unterstützt. Informationen zum Abfragen von Domänendiensteinträgen finden Sie im Thema [Domäne](domain.md).</span><span class="sxs-lookup"><span data-stu-id="c3bda-p102">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="c3bda-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c3bda-107">Properties</span></span>
| <span data-ttu-id="c3bda-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c3bda-108">Property</span></span>     | <span data-ttu-id="c3bda-109">Typ</span><span class="sxs-lookup"><span data-stu-id="c3bda-109">Type</span></span>   |<span data-ttu-id="c3bda-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c3bda-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3bda-111">id</span><span class="sxs-lookup"><span data-stu-id="c3bda-111">id</span></span>|<span data-ttu-id="c3bda-112">String</span><span class="sxs-lookup"><span data-stu-id="c3bda-112">String</span></span>| <span data-ttu-id="c3bda-p103">Eindeutiger Bezeichner, der dieser Entität zugewiesen ist. Lässt keine Nullwerte zu, schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c3bda-p103">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span> |
|<span data-ttu-id="c3bda-115">isOptional</span><span class="sxs-lookup"><span data-stu-id="c3bda-115">isOptional</span></span>|<span data-ttu-id="c3bda-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3bda-116">Boolean</span></span>| <span data-ttu-id="c3bda-117">Wenn „false“, muss der TXT-Eintrag vom Kunden auf dem DNS-Host konfiguriert werden, damit Microsoft-Onlinedienste ordnungsgemäß mit der Domäne funktionieren.</span><span class="sxs-lookup"><span data-stu-id="c3bda-117">If false, the TXT record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="c3bda-118">label</span><span class="sxs-lookup"><span data-stu-id="c3bda-118">label</span></span>|<span data-ttu-id="c3bda-119">String</span><span class="sxs-lookup"><span data-stu-id="c3bda-119">String</span></span>| <span data-ttu-id="c3bda-120">Wert, der beim Konfigurieren der *name*-Eigenschaft des TXT-Eintrags auf dem DNS-Host verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="c3bda-120">Value to use when configuring the *name* property of the TXT record at the DNS host.</span></span>|
|<span data-ttu-id="c3bda-121">recordType</span><span class="sxs-lookup"><span data-stu-id="c3bda-121">recordType</span></span>|<span data-ttu-id="c3bda-122">String</span><span class="sxs-lookup"><span data-stu-id="c3bda-122">String</span></span>| <span data-ttu-id="c3bda-p104">Typ des DNS-Eintrags. Der Wert ist immer *Txt*. Schlüssel</span><span class="sxs-lookup"><span data-stu-id="c3bda-p104">Type of DNS record. The value is always *Txt*. Key</span></span> |
|<span data-ttu-id="c3bda-126">supportedService</span><span class="sxs-lookup"><span data-stu-id="c3bda-126">supportedService</span></span>|<span data-ttu-id="c3bda-127">String</span><span class="sxs-lookup"><span data-stu-id="c3bda-127">String</span></span>| <span data-ttu-id="c3bda-128">Microsoft-Onlinedienst oder Feature mit Abhängigkeit von diesem TXT-Eintrag.</span><span class="sxs-lookup"><span data-stu-id="c3bda-128">Microsoft Online Service or feature that has a dependency on this TXT record.</span></span></br></br><span data-ttu-id="c3bda-129">Kann einer der folgenden Werte sein: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="c3bda-129">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="c3bda-130">text</span><span class="sxs-lookup"><span data-stu-id="c3bda-130">text</span></span>|<span data-ttu-id="c3bda-131">String</span><span class="sxs-lookup"><span data-stu-id="c3bda-131">String</span></span>| <span data-ttu-id="c3bda-132">Wert, der beim Konfigurieren der *text*-Eigenschaft auf dem DNS-Host verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="c3bda-132">Value used when configuring the *text* property at the DNS host.</span></span> |
|<span data-ttu-id="c3bda-133">ttl</span><span class="sxs-lookup"><span data-stu-id="c3bda-133">ttl</span></span>|<span data-ttu-id="c3bda-134">Int32</span><span class="sxs-lookup"><span data-stu-id="c3bda-134">Int32</span></span>| <span data-ttu-id="c3bda-p105">Wert, der beim Konfigurieren der Eigenschaft für die Gültigkeitsdauer (*time-to-live (ttl)*) des DNS-Eintrags auf dem DNS-Host verwendet werden soll. Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="c3bda-p105">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="c3bda-137">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c3bda-137">Relationships</span></span>
<span data-ttu-id="c3bda-138">Keine</span><span class="sxs-lookup"><span data-stu-id="c3bda-138">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c3bda-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c3bda-139">JSON representation</span></span>
<span data-ttu-id="c3bda-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c3bda-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsTxtRecord"
}-->

```json
{
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
  "description": "domainDnsTxtRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->