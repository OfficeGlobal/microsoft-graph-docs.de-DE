---
title: NetworkConnection Ressourcentyp
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: 7dfc055c7603adc8d60908df58ce3995927316cd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064315"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="1d817-104">NetworkConnection Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1d817-104">networkConnection resource type</span></span>

 > <span data-ttu-id="1d817-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1d817-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d817-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1d817-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1d817-107">Statusinformationen über die Netzwerkverbindung im Zusammenhang mit der Benachrichtigung enthält.</span><span class="sxs-lookup"><span data-stu-id="1d817-107">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="1d817-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1d817-108">Properties</span></span>

| <span data-ttu-id="1d817-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1d817-109">Property</span></span>   | <span data-ttu-id="1d817-110">Typ</span><span class="sxs-lookup"><span data-stu-id="1d817-110">Type</span></span>|<span data-ttu-id="1d817-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1d817-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d817-112">applicationName</span><span class="sxs-lookup"><span data-stu-id="1d817-112">applicationName</span></span>|<span data-ttu-id="1d817-113">String</span><span class="sxs-lookup"><span data-stu-id="1d817-113">String</span></span>|<span data-ttu-id="1d817-114">Name der Anwendung verwalten die Netzwerkschnittstelle (beispielsweise Facebook, SMTP, usw.).</span><span class="sxs-lookup"><span data-stu-id="1d817-114">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="1d817-115">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="1d817-115">destinationAddress</span></span>|<span data-ttu-id="1d817-116">String</span><span class="sxs-lookup"><span data-stu-id="1d817-116">String</span></span>|<span data-ttu-id="1d817-117">Ziel-IP-Adresse (der Verbindung).</span><span class="sxs-lookup"><span data-stu-id="1d817-117">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="1d817-118">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="1d817-118">destinationDomain</span></span>|<span data-ttu-id="1d817-119">String</span><span class="sxs-lookup"><span data-stu-id="1d817-119">String</span></span>|<span data-ttu-id="1d817-120">Ziel der Domänenteil der Ziel-URL.</span><span class="sxs-lookup"><span data-stu-id="1d817-120">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="1d817-121">(zum Beispiel "www.contoso.com").</span><span class="sxs-lookup"><span data-stu-id="1d817-121">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="1d817-122">destinationPort</span><span class="sxs-lookup"><span data-stu-id="1d817-122">destinationPort</span></span>|<span data-ttu-id="1d817-123">String</span><span class="sxs-lookup"><span data-stu-id="1d817-123">String</span></span>|<span data-ttu-id="1d817-124">Zielport (der Verbindung).</span><span class="sxs-lookup"><span data-stu-id="1d817-124">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="1d817-125">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="1d817-125">destinationUrl</span></span>|<span data-ttu-id="1d817-126">String</span><span class="sxs-lookup"><span data-stu-id="1d817-126">String</span></span>|<span data-ttu-id="1d817-127">Netzwerk-URL-URI-Verbindungszeichenfolge - Parameter ausschließen.</span><span class="sxs-lookup"><span data-stu-id="1d817-127">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="1d817-128">(zum Beispiel "www.contoso.com/products/default.html")</span><span class="sxs-lookup"><span data-stu-id="1d817-128">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="1d817-129">Richtung</span><span class="sxs-lookup"><span data-stu-id="1d817-129">direction</span></span>|<span data-ttu-id="1d817-130">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="1d817-130">connectionDirection</span></span>|<span data-ttu-id="1d817-131">Richtung der Netzwerk-Verbindung.</span><span class="sxs-lookup"><span data-stu-id="1d817-131">Network connection direction.</span></span> <span data-ttu-id="1d817-132">Mögliche Werte sind: `unknown`, `inbound` und `outbound`.</span><span class="sxs-lookup"><span data-stu-id="1d817-132">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="1d817-133">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="1d817-133">domainRegisteredDateTime</span></span>|<span data-ttu-id="1d817-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d817-134">DateTimeOffset</span></span>|<span data-ttu-id="1d817-135">Datum, wenn die Zieldomäne registriert wurde.</span><span class="sxs-lookup"><span data-stu-id="1d817-135">Date when the destination domain was registered.</span></span> <span data-ttu-id="1d817-136">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="1d817-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1d817-137">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="1d817-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="1d817-138">localDnsName</span><span class="sxs-lookup"><span data-stu-id="1d817-138">localDnsName</span></span>|<span data-ttu-id="1d817-139">String</span><span class="sxs-lookup"><span data-stu-id="1d817-139">String</span></span>|<span data-ttu-id="1d817-140">Der lokalen DNS-name Lösung, wie er in der Host lokalen DNS-Cache angezeigt wird (beispielsweise Fall, dass die Datei "Hosts" manipuliert wurde).</span><span class="sxs-lookup"><span data-stu-id="1d817-140">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="1d817-141">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="1d817-141">natDestinationAddress</span></span>|<span data-ttu-id="1d817-142">String</span><span class="sxs-lookup"><span data-stu-id="1d817-142">String</span></span>|<span data-ttu-id="1d817-143">Network Address Translation Ziel-IP-Adresse.</span><span class="sxs-lookup"><span data-stu-id="1d817-143">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="1d817-144">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="1d817-144">natDestinationPort</span></span>|<span data-ttu-id="1d817-145">String</span><span class="sxs-lookup"><span data-stu-id="1d817-145">String</span></span>|<span data-ttu-id="1d817-146">Network Address Translation Zielport.</span><span class="sxs-lookup"><span data-stu-id="1d817-146">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="1d817-147">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="1d817-147">natSourceAddress</span></span>|<span data-ttu-id="1d817-148">String</span><span class="sxs-lookup"><span data-stu-id="1d817-148">String</span></span>|<span data-ttu-id="1d817-149">Network Address Translation Quell-IP-Adresse.</span><span class="sxs-lookup"><span data-stu-id="1d817-149">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="1d817-150">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="1d817-150">natSourcePort</span></span>|<span data-ttu-id="1d817-151">String</span><span class="sxs-lookup"><span data-stu-id="1d817-151">String</span></span>|<span data-ttu-id="1d817-152">Network Address Translation Quellport.</span><span class="sxs-lookup"><span data-stu-id="1d817-152">Network Address Translation source port.</span></span>|
|<span data-ttu-id="1d817-153">protocol</span><span class="sxs-lookup"><span data-stu-id="1d817-153">protocol</span></span>|[<span data-ttu-id="1d817-154">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="1d817-154">securityNetworkProtocol</span></span>](securitynetworkprotocolenumtype.md)|<span data-ttu-id="1d817-155">Netzwerkprotokoll.</span><span class="sxs-lookup"><span data-stu-id="1d817-155">Network protocol.</span></span> <span data-ttu-id="1d817-156">Mögliche Werte sind: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd` , `raw`, `ipx`, `spx`, `spxII`.</span><span class="sxs-lookup"><span data-stu-id="1d817-156">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="1d817-157">riskScore</span><span class="sxs-lookup"><span data-stu-id="1d817-157">riskScore</span></span>|<span data-ttu-id="1d817-158">String</span><span class="sxs-lookup"><span data-stu-id="1d817-158">String</span></span>|<span data-ttu-id="1d817-159">Anbieter generiert/berechnet riskieren Bewertung der Verbindung.</span><span class="sxs-lookup"><span data-stu-id="1d817-159">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="1d817-160">Empfohlene Wertebereich von 0 bis 1, die den Prozentsatz entspricht.</span><span class="sxs-lookup"><span data-stu-id="1d817-160">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="1d817-161">sourceAddress</span><span class="sxs-lookup"><span data-stu-id="1d817-161">sourceAddress</span></span>|<span data-ttu-id="1d817-162">String</span><span class="sxs-lookup"><span data-stu-id="1d817-162">String</span></span>|<span data-ttu-id="1d817-163">Quelle (d. h. Ursprung) IP-Adresse (der Verbindung).</span><span class="sxs-lookup"><span data-stu-id="1d817-163">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="1d817-164">Quellport</span><span class="sxs-lookup"><span data-stu-id="1d817-164">sourcePort</span></span>|<span data-ttu-id="1d817-165">String</span><span class="sxs-lookup"><span data-stu-id="1d817-165">String</span></span>|<span data-ttu-id="1d817-166">Quelle (d. h. Ursprung) IP-Port (der Verbindung).</span><span class="sxs-lookup"><span data-stu-id="1d817-166">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="1d817-167">status</span><span class="sxs-lookup"><span data-stu-id="1d817-167">status</span></span>|<span data-ttu-id="1d817-168">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="1d817-168">connectionStatus</span></span>|<span data-ttu-id="1d817-169">Netzwerk-Verbindungsstatus.</span><span class="sxs-lookup"><span data-stu-id="1d817-169">Network connection status.</span></span> <span data-ttu-id="1d817-170">Mögliche Werte sind: `unknown`, `attempted`, `succeeded`, `blocked` und `failed`.</span><span class="sxs-lookup"><span data-stu-id="1d817-170">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="1d817-171">urlParameters</span><span class="sxs-lookup"><span data-stu-id="1d817-171">urlParameters</span></span>|<span data-ttu-id="1d817-172">String</span><span class="sxs-lookup"><span data-stu-id="1d817-172">String</span></span>|<span data-ttu-id="1d817-173">Parameter (Suffix) der Ziel-URL.</span><span class="sxs-lookup"><span data-stu-id="1d817-173">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1d817-174">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1d817-174">JSON representation</span></span>

<span data-ttu-id="1d817-175">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1d817-175">The following is a JSON representation of the resource.</span></span>

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
