---
title: NetworkConnection Ressourcentyp
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: ce7de8d5a0f63c4d924e8092e4e9e05f984ec335
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643587"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="b9a7a-104">NetworkConnection Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b9a7a-104">networkConnection resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9a7a-105">Statusinformationen über die Netzwerkverbindung im Zusammenhang mit der Benachrichtigung enthält.</span><span class="sxs-lookup"><span data-stu-id="b9a7a-105">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="b9a7a-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b9a7a-106">Properties</span></span>

| <span data-ttu-id="b9a7a-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b9a7a-107">Property</span></span>   | <span data-ttu-id="b9a7a-108">Typ</span><span class="sxs-lookup"><span data-stu-id="b9a7a-108">Type</span></span>|<span data-ttu-id="b9a7a-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9a7a-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9a7a-110">applicationName</span><span class="sxs-lookup"><span data-stu-id="b9a7a-110">applicationName</span></span>|<span data-ttu-id="b9a7a-111">String</span><span class="sxs-lookup"><span data-stu-id="b9a7a-111">String</span></span>|<span data-ttu-id="b9a7a-112">Name der Anwendung verwalten die Netzwerkschnittstelle (beispielsweise Facebook, SMTP, usw.).</span><span class="sxs-lookup"><span data-stu-id="b9a7a-112">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="b9a7a-113">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="b9a7a-113">destinationAddress</span></span>|<span data-ttu-id="b9a7a-114">String</span><span class="sxs-lookup"><span data-stu-id="b9a7a-114">String</span></span>|<span data-ttu-id="b9a7a-115">Ziel-IP-Adresse (der Verbindung).</span><span class="sxs-lookup"><span data-stu-id="b9a7a-115">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="b9a7a-116">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="b9a7a-116">destinationDomain</span></span>|<span data-ttu-id="b9a7a-117">String</span><span class="sxs-lookup"><span data-stu-id="b9a7a-117">String</span></span>|<span data-ttu-id="b9a7a-118">Ziel der Domänenteil der Ziel-URL.</span><span class="sxs-lookup"><span data-stu-id="b9a7a-118">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="b9a7a-119">(zum Beispiel "www.contoso.com").</span><span class="sxs-lookup"><span data-stu-id="b9a7a-119">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="b9a7a-120">destinationPort</span><span class="sxs-lookup"><span data-stu-id="b9a7a-120">destinationPort</span></span>|<span data-ttu-id="b9a7a-121">String</span><span class="sxs-lookup"><span data-stu-id="b9a7a-121">String</span></span>|<span data-ttu-id="b9a7a-122">Zielport (der Verbindung).</span><span class="sxs-lookup"><span data-stu-id="b9a7a-122">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="b9a7a-123">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="b9a7a-123">destinationUrl</span></span>|<span data-ttu-id="b9a7a-124">String</span><span class="sxs-lookup"><span data-stu-id="b9a7a-124">String</span></span>|<span data-ttu-id="b9a7a-125">Netzwerk-URL-URI-Verbindungszeichenfolge - Parameter ausschließen.</span><span class="sxs-lookup"><span data-stu-id="b9a7a-125">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="b9a7a-126">(zum Beispiel "www.contoso.com/products/default.html")</span><span class="sxs-lookup"><span data-stu-id="b9a7a-126">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="b9a7a-127">direction</span><span class="sxs-lookup"><span data-stu-id="b9a7a-127">direction</span></span>|<span data-ttu-id="b9a7a-128">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="b9a7a-128">connectionDirection</span></span>|<span data-ttu-id="b9a7a-129">Richtung der Netzwerk-Verbindung.</span><span class="sxs-lookup"><span data-stu-id="b9a7a-129">Network connection direction.</span></span> <span data-ttu-id="b9a7a-130">Mögliche Werte sind: `unknown`, `inbound` und `outbound`.</span><span class="sxs-lookup"><span data-stu-id="b9a7a-130">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="b9a7a-131">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="b9a7a-131">domainRegisteredDateTime</span></span>|<span data-ttu-id="b9a7a-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9a7a-132">DateTimeOffset</span></span>|<span data-ttu-id="b9a7a-133">Datum, wenn die Zieldomäne registriert wurde.</span><span class="sxs-lookup"><span data-stu-id="b9a7a-133">Date when the destination domain was registered.</span></span> <span data-ttu-id="b9a7a-134">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="b9a7a-134">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b9a7a-135">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b9a7a-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b9a7a-136">localDnsName</span><span class="sxs-lookup"><span data-stu-id="b9a7a-136">localDnsName</span></span>|<span data-ttu-id="b9a7a-137">String</span><span class="sxs-lookup"><span data-stu-id="b9a7a-137">String</span></span>|<span data-ttu-id="b9a7a-138">Der lokalen DNS-name Lösung, wie er in der Host lokalen DNS-Cache angezeigt wird (beispielsweise Fall, dass die Datei "Hosts" manipuliert wurde).</span><span class="sxs-lookup"><span data-stu-id="b9a7a-138">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="b9a7a-139">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="b9a7a-139">natDestinationAddress</span></span>|<span data-ttu-id="b9a7a-140">String</span><span class="sxs-lookup"><span data-stu-id="b9a7a-140">String</span></span>|<span data-ttu-id="b9a7a-141">Network Address Translation Ziel-IP-Adresse.</span><span class="sxs-lookup"><span data-stu-id="b9a7a-141">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="b9a7a-142">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="b9a7a-142">natDestinationPort</span></span>|<span data-ttu-id="b9a7a-143">String</span><span class="sxs-lookup"><span data-stu-id="b9a7a-143">String</span></span>|<span data-ttu-id="b9a7a-144">Network Address Translation Zielport.</span><span class="sxs-lookup"><span data-stu-id="b9a7a-144">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="b9a7a-145">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="b9a7a-145">natSourceAddress</span></span>|<span data-ttu-id="b9a7a-146">String</span><span class="sxs-lookup"><span data-stu-id="b9a7a-146">String</span></span>|<span data-ttu-id="b9a7a-147">Network Address Translation Quell-IP-Adresse.</span><span class="sxs-lookup"><span data-stu-id="b9a7a-147">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="b9a7a-148">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="b9a7a-148">natSourcePort</span></span>|<span data-ttu-id="b9a7a-149">String</span><span class="sxs-lookup"><span data-stu-id="b9a7a-149">String</span></span>|<span data-ttu-id="b9a7a-150">Network Address Translation Quellport.</span><span class="sxs-lookup"><span data-stu-id="b9a7a-150">Network Address Translation source port.</span></span>|
|<span data-ttu-id="b9a7a-151">protocol</span><span class="sxs-lookup"><span data-stu-id="b9a7a-151">protocol</span></span>|[<span data-ttu-id="b9a7a-152">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="b9a7a-152">securityNetworkProtocol</span></span>](securitynetworkprotocolenumtype.md)|<span data-ttu-id="b9a7a-153">Netzwerkprotokoll.</span><span class="sxs-lookup"><span data-stu-id="b9a7a-153">Network protocol.</span></span> <span data-ttu-id="b9a7a-154">Mögliche Werte sind: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd` , `raw`, `ipx`, `spx`, `spxII`.</span><span class="sxs-lookup"><span data-stu-id="b9a7a-154">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="b9a7a-155">riskScore</span><span class="sxs-lookup"><span data-stu-id="b9a7a-155">riskScore</span></span>|<span data-ttu-id="b9a7a-156">String</span><span class="sxs-lookup"><span data-stu-id="b9a7a-156">String</span></span>|<span data-ttu-id="b9a7a-157">Anbieter generiert/berechnet riskieren Bewertung der Verbindung.</span><span class="sxs-lookup"><span data-stu-id="b9a7a-157">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="b9a7a-158">Empfohlene Wertebereich von 0 bis 1, die den Prozentsatz entspricht.</span><span class="sxs-lookup"><span data-stu-id="b9a7a-158">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="b9a7a-159">sourceAddress</span><span class="sxs-lookup"><span data-stu-id="b9a7a-159">sourceAddress</span></span>|<span data-ttu-id="b9a7a-160">String</span><span class="sxs-lookup"><span data-stu-id="b9a7a-160">String</span></span>|<span data-ttu-id="b9a7a-161">Quelle (d. h. Ursprung) IP-Adresse (der Verbindung).</span><span class="sxs-lookup"><span data-stu-id="b9a7a-161">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="b9a7a-162">Quellport</span><span class="sxs-lookup"><span data-stu-id="b9a7a-162">sourcePort</span></span>|<span data-ttu-id="b9a7a-163">String</span><span class="sxs-lookup"><span data-stu-id="b9a7a-163">String</span></span>|<span data-ttu-id="b9a7a-164">Quelle (d. h. Ursprung) IP-Port (der Verbindung).</span><span class="sxs-lookup"><span data-stu-id="b9a7a-164">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="b9a7a-165">status</span><span class="sxs-lookup"><span data-stu-id="b9a7a-165">status</span></span>|<span data-ttu-id="b9a7a-166">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="b9a7a-166">connectionStatus</span></span>|<span data-ttu-id="b9a7a-167">Netzwerk-Verbindungsstatus.</span><span class="sxs-lookup"><span data-stu-id="b9a7a-167">Network connection status.</span></span> <span data-ttu-id="b9a7a-168">Mögliche Werte: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="b9a7a-168">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="b9a7a-169">urlParameters</span><span class="sxs-lookup"><span data-stu-id="b9a7a-169">urlParameters</span></span>|<span data-ttu-id="b9a7a-170">String</span><span class="sxs-lookup"><span data-stu-id="b9a7a-170">String</span></span>|<span data-ttu-id="b9a7a-171">Parameter (Suffix) der Ziel-URL.</span><span class="sxs-lookup"><span data-stu-id="b9a7a-171">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b9a7a-172">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b9a7a-172">JSON representation</span></span>

<span data-ttu-id="b9a7a-173">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b9a7a-173">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "networkConnection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/networkconnection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
