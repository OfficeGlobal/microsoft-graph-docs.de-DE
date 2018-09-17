# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="3afa9-101">Ressourcentyp hostSecurityState</span><span class="sxs-lookup"><span data-stu-id="3afa9-101">hostSecurityState resource type</span></span>

<span data-ttu-id="3afa9-102">Enthält Zustandsinformationen über den Host (einschließlich der Geräte, Computer und usw.).</span><span class="sxs-lookup"><span data-stu-id="3afa9-102">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="3afa9-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3afa9-103">Properties</span></span>

| <span data-ttu-id="3afa9-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3afa9-104">Property</span></span>   | <span data-ttu-id="3afa9-105">Typ</span><span class="sxs-lookup"><span data-stu-id="3afa9-105">Type</span></span>|<span data-ttu-id="3afa9-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3afa9-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3afa9-107">fqdn</span><span class="sxs-lookup"><span data-stu-id="3afa9-107">FQDN</span></span>|<span data-ttu-id="3afa9-108">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3afa9-108">String</span></span>|<span data-ttu-id="3afa9-109">Host FQDN (Fully Qualified Domain Name) (z.B. `machine.company.com`).</span><span class="sxs-lookup"><span data-stu-id="3afa9-109">Host FQDN (Fully Qualified Domain Name) (for example, `machine.company.com`).</span></span>|
|<span data-ttu-id="3afa9-110">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="3afa9-110">isAzureAadJoined</span></span>|<span data-ttu-id="3afa9-111">Boolesch</span><span class="sxs-lookup"><span data-stu-id="3afa9-111">Boolean</span></span>|<span data-ttu-id="3afa9-112">True, wenn der Host Teil der Azure Active Directory Domain Services ist.</span><span class="sxs-lookup"><span data-stu-id="3afa9-112">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="3afa9-113">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="3afa9-113">isAzureAadRegistered</span></span>|<span data-ttu-id="3afa9-114">Boolesch</span><span class="sxs-lookup"><span data-stu-id="3afa9-114">Boolean</span></span>|<span data-ttu-id="3afa9-115">True, wenn der Host mit der Azure Active Directory Gerät-Registrierung (BYOD Geräte - d.h., nicht vollständig durch Enterprise verwaltet) registriert ist.</span><span class="sxs-lookup"><span data-stu-id="3afa9-115">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="3afa9-116">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="3afa9-116">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="3afa9-117">Boolesch</span><span class="sxs-lookup"><span data-stu-id="3afa9-117">Boolean</span></span>|<span data-ttu-id="3afa9-118">True, wenn der Host der Domäne mit einer lokalen Active Directory-Domäne verbunden ist.</span><span class="sxs-lookup"><span data-stu-id="3afa9-118">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="3afa9-119">netBiosName</span><span class="sxs-lookup"><span data-stu-id="3afa9-119">netBiosName</span></span>|<span data-ttu-id="3afa9-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3afa9-120">String</span></span>|<span data-ttu-id="3afa9-121">Der Name der lokalen Host ohne den DNS-Domänennamen.</span><span class="sxs-lookup"><span data-stu-id="3afa9-121">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="3afa9-122">os</span><span class="sxs-lookup"><span data-stu-id="3afa9-122">OS</span></span>|<span data-ttu-id="3afa9-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3afa9-123">String</span></span>|<span data-ttu-id="3afa9-124">Hostbetriebssystem.</span><span class="sxs-lookup"><span data-stu-id="3afa9-124">Host Operating System.</span></span> <span data-ttu-id="3afa9-125">(Z.B. Windows10, Mac OS, RHEL, usw.).</span><span class="sxs-lookup"><span data-stu-id="3afa9-125">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="3afa9-126">privateIpAddress</span><span class="sxs-lookup"><span data-stu-id="3afa9-126">privateIpAddress</span></span>|<span data-ttu-id="3afa9-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3afa9-127">String</span></span>|<span data-ttu-id="3afa9-128">Private (nicht-routingfähige) IPv4- oder IPv6-Adresse (siehe [RFC 1918](https://tools.ietf.org/html/rfc1918)) zum Zeitpunkt der Warnung.</span><span class="sxs-lookup"><span data-stu-id="3afa9-128">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="3afa9-129">publicIpAddress</span><span class="sxs-lookup"><span data-stu-id="3afa9-129">publicIpAddress</span></span>|<span data-ttu-id="3afa9-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3afa9-130">String</span></span>|<span data-ttu-id="3afa9-131">Öffentliche routingfähige IPv4- oder IPv6-Adresse (siehe [RFC 1918](https://tools.ietf.org/html/rfc1918)) zum Zeitpunkt der Warnung.</span><span class="sxs-lookup"><span data-stu-id="3afa9-131">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="3afa9-132">riskScore</span><span class="sxs-lookup"><span data-stu-id="3afa9-132">riskScore</span></span>|<span data-ttu-id="3afa9-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3afa9-133">String</span></span>|<span data-ttu-id="3afa9-134">Vom Anbieter generierte/berechnete Risikobewertung des Hosts.</span><span class="sxs-lookup"><span data-stu-id="3afa9-134">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="3afa9-135">Empfohlener Wertebereich von 0-1, was einem Prozentsatz entspricht.</span><span class="sxs-lookup"><span data-stu-id="3afa9-135">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3afa9-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3afa9-136">JSON representation</span></span>

<span data-ttu-id="3afa9-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3afa9-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.hostSecurityState"
}-->

```json
{
  "fqdn": "String",
  "isAzureAadJoined": true,
  "isAzureAadRegistered": true,
  "isHybridAzureDomainJoined": true,
  "netBiosName": "String",
  "os": "String",
  "privateIpAddress": "String",
  "publicIpAddress": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "hostSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
