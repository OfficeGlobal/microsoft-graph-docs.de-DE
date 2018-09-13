# <a name="networkconnection-resource-type"></a><span data-ttu-id="8a3ef-101">networkConnection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8a3ef-101">networkConnection resource type</span></span>

<span data-ttu-id="8a3ef-102">Enthält zustandsbehaftete Informationen zur Netzwerkverbindung, die sich auf die Warnung beziehen.</span><span class="sxs-lookup"><span data-stu-id="8a3ef-102">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="8a3ef-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8a3ef-103">Properties</span></span>

| <span data-ttu-id="8a3ef-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8a3ef-104">Property</span></span>   | <span data-ttu-id="8a3ef-105">Typ</span><span class="sxs-lookup"><span data-stu-id="8a3ef-105">Type</span></span>|<span data-ttu-id="8a3ef-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8a3ef-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a3ef-107">applicationName</span><span class="sxs-lookup"><span data-stu-id="8a3ef-107">applicationName</span></span>|<span data-ttu-id="8a3ef-108">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8a3ef-108">String</span></span>|<span data-ttu-id="8a3ef-109">Name der Anwendung, die die Netzwerkverbindung verwaltet (z. B. Facebook, SMTP usw.).</span><span class="sxs-lookup"><span data-stu-id="8a3ef-109">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="8a3ef-110">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="8a3ef-110">destinationAddress</span></span>|<span data-ttu-id="8a3ef-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8a3ef-111">String</span></span>|<span data-ttu-id="8a3ef-112">Ziel-IP-Adresse (der Netzwerkverbindung).</span><span class="sxs-lookup"><span data-stu-id="8a3ef-112">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="8a3ef-113">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="8a3ef-113">destinationDomain</span></span>|<span data-ttu-id="8a3ef-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8a3ef-114">String</span></span>|<span data-ttu-id="8a3ef-115">Zieldomänenteil der Ziel-URL.</span><span class="sxs-lookup"><span data-stu-id="8a3ef-115">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="8a3ef-116">(zum Beispiel "www.contoso.com").</span><span class="sxs-lookup"><span data-stu-id="8a3ef-116">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="8a3ef-117">destinationPort</span><span class="sxs-lookup"><span data-stu-id="8a3ef-117">destinationPort</span></span>|<span data-ttu-id="8a3ef-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8a3ef-118">String</span></span>|<span data-ttu-id="8a3ef-119">Zielport (der Netzwerkverbindung).</span><span class="sxs-lookup"><span data-stu-id="8a3ef-119">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="8a3ef-120">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="8a3ef-120">destinationUrl</span></span>|<span data-ttu-id="8a3ef-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8a3ef-121">String</span></span>|<span data-ttu-id="8a3ef-122">Netzwerkverbindungs-URL / URI-Zeichenfolge - ohne Parameter.</span><span class="sxs-lookup"><span data-stu-id="8a3ef-122">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="8a3ef-123">(zum Beispiel "www.contoso.com/products/default.html")</span><span class="sxs-lookup"><span data-stu-id="8a3ef-123">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="8a3ef-124">Richtung</span><span class="sxs-lookup"><span data-stu-id="8a3ef-124">direction</span></span>|<span data-ttu-id="8a3ef-125">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="8a3ef-125">connectionDirection</span></span>|<span data-ttu-id="8a3ef-126">Richtung der Netzwerkverbindung.</span><span class="sxs-lookup"><span data-stu-id="8a3ef-126">Network connection direction.</span></span> <span data-ttu-id="8a3ef-127">Mögliche Werte sind: `unknown`, `inbound` und `outbound`.</span><span class="sxs-lookup"><span data-stu-id="8a3ef-127">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="8a3ef-128">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="8a3ef-128">domainRegisteredDateTime</span></span>|<span data-ttu-id="8a3ef-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a3ef-129">DateTimeOffset</span></span>|<span data-ttu-id="8a3ef-130">Datum, an dem die Zieldomäne registriert wurde.</span><span class="sxs-lookup"><span data-stu-id="8a3ef-130">Date when the destination domain was registered.</span></span> <span data-ttu-id="8a3ef-131">Der Zeitstempel-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="8a3ef-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8a3ef-132">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="8a3ef-132">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="8a3ef-133">localDnsName</span><span class="sxs-lookup"><span data-stu-id="8a3ef-133">localDnsName</span></span>|<span data-ttu-id="8a3ef-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8a3ef-134">String</span></span>|<span data-ttu-id="8a3ef-135">Die lokale DNS-Namensauflösung, die im lokalen DNS-Cache des Hosts angezeigt wird (z. B. für den Fall, dass die Datei "hosts" manipuliert wurde).</span><span class="sxs-lookup"><span data-stu-id="8a3ef-135">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="8a3ef-136">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="8a3ef-136">natDestinationAddress</span></span>|<span data-ttu-id="8a3ef-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8a3ef-137">String</span></span>|<span data-ttu-id="8a3ef-138">Netzwerkadressenübersetzung Ziel-IP-Adresse.</span><span class="sxs-lookup"><span data-stu-id="8a3ef-138">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="8a3ef-139">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="8a3ef-139">natDestinationPort</span></span>|<span data-ttu-id="8a3ef-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8a3ef-140">String</span></span>|<span data-ttu-id="8a3ef-141">Netzwerkadressenübersetzung Zielport.</span><span class="sxs-lookup"><span data-stu-id="8a3ef-141">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="8a3ef-142">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="8a3ef-142">natSourceAddress</span></span>|<span data-ttu-id="8a3ef-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8a3ef-143">String</span></span>|<span data-ttu-id="8a3ef-144">Netzwerkadressenübersetzung Ursprungs-IP-Adresse.</span><span class="sxs-lookup"><span data-stu-id="8a3ef-144">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="8a3ef-145">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="8a3ef-145">natSourcePort</span></span>|<span data-ttu-id="8a3ef-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8a3ef-146">String</span></span>|<span data-ttu-id="8a3ef-147">Netzwerkadressenübersetzung Quellport.</span><span class="sxs-lookup"><span data-stu-id="8a3ef-147">Network Address Translation source port.</span></span>|
|<span data-ttu-id="8a3ef-148">Protokoll</span><span class="sxs-lookup"><span data-stu-id="8a3ef-148">protocol</span></span>|[<span data-ttu-id="8a3ef-149">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="8a3ef-149">securityNetworkProtocol</span></span>](securitynetworkprotocol.md)|<span data-ttu-id="8a3ef-150">Netzwerkprotokoll</span><span class="sxs-lookup"><span data-stu-id="8a3ef-150">Network protocol analysis</span></span> <span data-ttu-id="8a3ef-151">Mögliche Werte sind: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span><span class="sxs-lookup"><span data-stu-id="8a3ef-151">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`.</span></span>|
|<span data-ttu-id="8a3ef-152">riskScore</span><span class="sxs-lookup"><span data-stu-id="8a3ef-152">riskScore</span></span>|<span data-ttu-id="8a3ef-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8a3ef-153">String</span></span>|<span data-ttu-id="8a3ef-154">Vom Provider generierte / berechnete Risikobewertung der Netzwerkverbindung.</span><span class="sxs-lookup"><span data-stu-id="8a3ef-154">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="8a3ef-155">Empfohlener Wertebereich von 0-1, was einem Prozentsatz entspricht.</span><span class="sxs-lookup"><span data-stu-id="8a3ef-155">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="8a3ef-156">SourceAddress</span><span class="sxs-lookup"><span data-stu-id="8a3ef-156">sourceAddress</span></span>|<span data-ttu-id="8a3ef-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8a3ef-157">String</span></span>|<span data-ttu-id="8a3ef-158">Quell- (d. h. Ursprung) IP-Adresse (der Netzwerkverbindung).</span><span class="sxs-lookup"><span data-stu-id="8a3ef-158">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="8a3ef-159">sourcePort</span><span class="sxs-lookup"><span data-stu-id="8a3ef-159">sourcePort</span></span>|<span data-ttu-id="8a3ef-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8a3ef-160">String</span></span>|<span data-ttu-id="8a3ef-161">Quelle (d. h. Ursprung) IP-Port (der Netzwerkverbindung).</span><span class="sxs-lookup"><span data-stu-id="8a3ef-161">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="8a3ef-162">Status</span><span class="sxs-lookup"><span data-stu-id="8a3ef-162">status</span></span>|<span data-ttu-id="8a3ef-163">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="8a3ef-163">ConnectionStatus</span></span>|<span data-ttu-id="8a3ef-164">Status der Netzwerkverbinung</span><span class="sxs-lookup"><span data-stu-id="8a3ef-164">Network connection status.</span></span> <span data-ttu-id="8a3ef-165">Mögliche Werte: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="8a3ef-165">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="8a3ef-166">urlParameters</span><span class="sxs-lookup"><span data-stu-id="8a3ef-166">urlParameters</span></span>|<span data-ttu-id="8a3ef-167">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8a3ef-167">String</span></span>|<span data-ttu-id="8a3ef-168">Parameter (Suffix) der Ziel-URL.</span><span class="sxs-lookup"><span data-stu-id="8a3ef-168">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8a3ef-169">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8a3ef-169">JSON representation</span></span>

<span data-ttu-id="8a3ef-170">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8a3ef-170">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkConnection"
}-->

```json
{
  "applicationName": "String",
  "destinationAddress": "String",
  "destinationDomain": "String",
  "destinationPort": "String",
  "destinationUrl": "String",
  "direction": "@odata.type: microsoft.graph.connectionDirection",
  "domainRegisteredDateTime": "String (timestamp)",
  "localDnsName": "String",
  "natDestinationAddress": "String",
  "natDestinationPort": "String",
  "natSourceAddress": "String",
  "natSourcePort": "String",
  "protocol": "@odata.type: microsoft.graph.securityNetworkProtocol",
  "riskScore": "String",
  "sourceAddress": "String",
  "sourcePort": "String",
  "status": "@odata.type: microsoft.graph.connectionStatus",
  "urlParameters": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkConnection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->