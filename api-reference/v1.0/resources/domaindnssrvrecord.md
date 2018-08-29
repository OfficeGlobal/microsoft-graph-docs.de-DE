# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="0d1b7-101">domainDnsSrvRecord-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0d1b7-101">domainDnsSrvRecord resource type</span></span>

<span data-ttu-id="0d1b7-p101">Stellt einen SRV-Eintrag dar, der der DNS-Zonendatei einer bestimmten Domäne im Mandanten hinzugefügt wird. Geerbt von der Entität [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="0d1b7-p101">Represents a SRV record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="0d1b7-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="0d1b7-104">Methods</span></span>
<span data-ttu-id="0d1b7-p102">Direkte Abfragen dieser Ressource werden nicht unterstützt. Informationen zum Abfragen von Domänendiensteinträgen finden Sie im Thema [Domäne](domain.md).</span><span class="sxs-lookup"><span data-stu-id="0d1b7-p102">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="0d1b7-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0d1b7-107">Properties</span></span>
| <span data-ttu-id="0d1b7-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0d1b7-108">Property</span></span>     | <span data-ttu-id="0d1b7-109">Typ</span><span class="sxs-lookup"><span data-stu-id="0d1b7-109">Type</span></span>   |<span data-ttu-id="0d1b7-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0d1b7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d1b7-111">id</span><span class="sxs-lookup"><span data-stu-id="0d1b7-111">id</span></span>|<span data-ttu-id="0d1b7-112">String</span><span class="sxs-lookup"><span data-stu-id="0d1b7-112">String</span></span>| <span data-ttu-id="0d1b7-p103">Eindeutiger Bezeichner, der dieser Entität zugewiesen ist. Lässt keine Nullwerte zu, schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0d1b7-p103">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="0d1b7-115">isOptional</span><span class="sxs-lookup"><span data-stu-id="0d1b7-115">isOptional</span></span>|<span data-ttu-id="0d1b7-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d1b7-116">Boolean</span></span>| <span data-ttu-id="0d1b7-117">Wenn „false“, muss der SRV-Eintrag vom Kunden auf dem DNS-Host konfiguriert werden, damit Microsoft-Onlinedienste ordnungsgemäß mit der Domäne funktionieren.</span><span class="sxs-lookup"><span data-stu-id="0d1b7-117">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="0d1b7-118">label</span><span class="sxs-lookup"><span data-stu-id="0d1b7-118">label</span></span>|<span data-ttu-id="0d1b7-119">String</span><span class="sxs-lookup"><span data-stu-id="0d1b7-119">String</span></span>| <span data-ttu-id="0d1b7-120">Wert, der beim Konfigurieren der *name*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="0d1b7-120">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="0d1b7-121">nameTarget</span><span class="sxs-lookup"><span data-stu-id="0d1b7-121">nameTarget</span></span>|<span data-ttu-id="0d1b7-122">String</span><span class="sxs-lookup"><span data-stu-id="0d1b7-122">String</span></span>| <span data-ttu-id="0d1b7-123">Wert, der beim Konfigurieren der *target*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="0d1b7-123">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="0d1b7-124">port</span><span class="sxs-lookup"><span data-stu-id="0d1b7-124">port</span></span>|<span data-ttu-id="0d1b7-125">Int32</span><span class="sxs-lookup"><span data-stu-id="0d1b7-125">Int32</span></span>| <span data-ttu-id="0d1b7-126">Wert, der beim Konfigurieren der *port*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="0d1b7-126">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="0d1b7-127">priority</span><span class="sxs-lookup"><span data-stu-id="0d1b7-127">priority</span></span>|<span data-ttu-id="0d1b7-128">Int32</span><span class="sxs-lookup"><span data-stu-id="0d1b7-128">Int32</span></span>| <span data-ttu-id="0d1b7-129">Wert, der beim Konfigurieren der *priority*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="0d1b7-129">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="0d1b7-130">protocol</span><span class="sxs-lookup"><span data-stu-id="0d1b7-130">protocol</span></span>|<span data-ttu-id="0d1b7-131">String</span><span class="sxs-lookup"><span data-stu-id="0d1b7-131">String</span></span>| <span data-ttu-id="0d1b7-132">Wert, der beim Konfigurieren der *protocol*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="0d1b7-132">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="0d1b7-133">recordType</span><span class="sxs-lookup"><span data-stu-id="0d1b7-133">recordType</span></span>|<span data-ttu-id="0d1b7-134">String</span><span class="sxs-lookup"><span data-stu-id="0d1b7-134">String</span></span>|  <span data-ttu-id="0d1b7-p104">Typ des DNS-Eintrags. Der Wert ist immer *Srv*. Schlüssel</span><span class="sxs-lookup"><span data-stu-id="0d1b7-p104">Type of DNS record. The value is always *Srv*. Key</span></span> |
|<span data-ttu-id="0d1b7-138">service</span><span class="sxs-lookup"><span data-stu-id="0d1b7-138">service</span></span>|<span data-ttu-id="0d1b7-139">String</span><span class="sxs-lookup"><span data-stu-id="0d1b7-139">String</span></span>| <span data-ttu-id="0d1b7-140">Wert, der beim Konfigurieren der *service*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="0d1b7-140">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="0d1b7-141">supportedService</span><span class="sxs-lookup"><span data-stu-id="0d1b7-141">supportedService</span></span>|<span data-ttu-id="0d1b7-142">String</span><span class="sxs-lookup"><span data-stu-id="0d1b7-142">String</span></span>| <span data-ttu-id="0d1b7-143">Microsoft-Onlinedienst oder Feature mit Abhängigkeit von diesem SRV-Eintrag.</span><span class="sxs-lookup"><span data-stu-id="0d1b7-143">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="0d1b7-144">Kann einer der folgenden Werte sein: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="0d1b7-144">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="0d1b7-145">ttl</span><span class="sxs-lookup"><span data-stu-id="0d1b7-145">ttl</span></span>|<span data-ttu-id="0d1b7-146">Int32</span><span class="sxs-lookup"><span data-stu-id="0d1b7-146">Int32</span></span>| <span data-ttu-id="0d1b7-p105">Wert, der beim Konfigurieren der Eigenschaft für die Gültigkeitsdauer (*time-to-live (ttl)*) des SRV-Eintrags auf dem DNS-Host verwendet werden soll. Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="0d1b7-p105">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host. Not nullable</span></span> |
|<span data-ttu-id="0d1b7-149">weight</span><span class="sxs-lookup"><span data-stu-id="0d1b7-149">weight</span></span>|<span data-ttu-id="0d1b7-150">Int32</span><span class="sxs-lookup"><span data-stu-id="0d1b7-150">Int32</span></span>| <span data-ttu-id="0d1b7-151">Wert, der beim Konfigurieren der *weight*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="0d1b7-151">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0d1b7-152">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0d1b7-152">Relationships</span></span>
<span data-ttu-id="0d1b7-153">Keine</span><span class="sxs-lookup"><span data-stu-id="0d1b7-153">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0d1b7-154">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0d1b7-154">JSON representation</span></span>
<span data-ttu-id="0d1b7-155">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0d1b7-155">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsSrvRecord"
}-->

```json
{
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "nameTarget": "String",
  "port": 1024,
  "priority": 1024,
  "protocol": "String",
  "recordType": "String",
  "service": "String",
  "supportedService": "String",
  "ttl": 1024,
  "weight": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsSrvRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->