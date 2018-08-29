# <a name="domaindnscnamerecord-resource-type"></a><span data-ttu-id="88775-101">domainDnsCnameRecord-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="88775-101">domainDnsCnameRecord resource type</span></span>

<span data-ttu-id="88775-p101">Stellt einen CNAME-Eintrag dar, der der DNS-Zonendatei einer bestimmten Domäne im Mandanten hinzugefügt wird. Geerbt von der Entität [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="88775-p101">Represents a CNAME record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>


## <a name="methods"></a><span data-ttu-id="88775-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="88775-104">Methods</span></span>
<span data-ttu-id="88775-p102">Direkte Abfragen dieser Ressource werden nicht unterstützt. Informationen zum Abfragen von Domänendiensteinträgen finden Sie im Thema [Domäne](domain.md).</span><span class="sxs-lookup"><span data-stu-id="88775-p102">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="88775-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="88775-107">Properties</span></span>
| <span data-ttu-id="88775-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="88775-108">Property</span></span>     | <span data-ttu-id="88775-109">Typ</span><span class="sxs-lookup"><span data-stu-id="88775-109">Type</span></span>   |<span data-ttu-id="88775-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="88775-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88775-111">canonicalName</span><span class="sxs-lookup"><span data-stu-id="88775-111">canonicalName</span></span>|<span data-ttu-id="88775-112">String</span><span class="sxs-lookup"><span data-stu-id="88775-112">String</span></span>| <span data-ttu-id="88775-p103">Der kanonische Name des CNAME-Eintrags. Wird verwendet, um den CNAME-Eintrag auf dem DNS-Host zu konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="88775-p103">The canonical name of the CNAME record. Used to configure the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="88775-115">id</span><span class="sxs-lookup"><span data-stu-id="88775-115">id</span></span>|<span data-ttu-id="88775-116">String</span><span class="sxs-lookup"><span data-stu-id="88775-116">String</span></span>| <span data-ttu-id="88775-p104">Eindeutiger Bezeichner, der dieser Entität zugewiesen ist. Lässt keine Nullwerte zu, schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="88775-p104">Unique identifier assigned to this entity. Not nullable, Read-only</span></span>|
|<span data-ttu-id="88775-119">isOptional</span><span class="sxs-lookup"><span data-stu-id="88775-119">isOptional</span></span>|<span data-ttu-id="88775-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="88775-120">Boolean</span></span>| <span data-ttu-id="88775-p105">Wenn „false“, muss der CNAME-Eintrag vom Kunden auf dem DNS-Host konfiguriert werden, damit Microsoft-Onlinedienste ordnungsgemäß mit der Domäne funktionieren. Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="88775-p105">If false, the CNAME record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain. Not nullable</span></span> |
|<span data-ttu-id="88775-123">label</span><span class="sxs-lookup"><span data-stu-id="88775-123">label</span></span>|<span data-ttu-id="88775-124">String</span><span class="sxs-lookup"><span data-stu-id="88775-124">String</span></span>| <span data-ttu-id="88775-125">Wert, der beim Konfigurieren der *alias/host/name*-Eigenschaft des CNAME-Eintrags auf dem DNS-Host verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="88775-125">Value used when configuring the *alias/host/name* of the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="88775-126">recordType</span><span class="sxs-lookup"><span data-stu-id="88775-126">recordType</span></span>|<span data-ttu-id="88775-127">String</span><span class="sxs-lookup"><span data-stu-id="88775-127">String</span></span>| <span data-ttu-id="88775-p106">Typ des DNS-Eintrags. Der Wert ist immer *CName*. Schlüssel</span><span class="sxs-lookup"><span data-stu-id="88775-p106">Type of DNS record. The value is always *CName*. Key</span></span>|
|<span data-ttu-id="88775-131">supportedService</span><span class="sxs-lookup"><span data-stu-id="88775-131">supportedService</span></span>|<span data-ttu-id="88775-132">String</span><span class="sxs-lookup"><span data-stu-id="88775-132">String</span></span>| <span data-ttu-id="88775-133">Microsoft-Onlinedienst oder Feature mit Abhängigkeit von diesem CNAME-Eintrag.</span><span class="sxs-lookup"><span data-stu-id="88775-133">Microsoft Online Service or feature that has a dependency on this CNAME record.</span></span></br></br><span data-ttu-id="88775-134">Kann einer der folgenden Werte sein: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="88775-134">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="88775-135">ttl</span><span class="sxs-lookup"><span data-stu-id="88775-135">ttl</span></span>|<span data-ttu-id="88775-136">Int32</span><span class="sxs-lookup"><span data-stu-id="88775-136">Int32</span></span>| <span data-ttu-id="88775-p107">Wert, der beim Konfigurieren der Eigenschaft für die Gültigkeitsdauer (time-to-live (ttl) des CNAME-Eintrags auf dem DNS-Host verwendet werden soll. Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="88775-p107">Value to use when configuring the time-to-live (ttl) property of the CNAME record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="88775-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="88775-139">Relationships</span></span>
<span data-ttu-id="88775-140">Keine</span><span class="sxs-lookup"><span data-stu-id="88775-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="88775-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="88775-141">JSON representation</span></span>
<span data-ttu-id="88775-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="88775-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsCnameRecord"
}-->

```json
{
  "canonicalName": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsCnameRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->