---
title: NetworkConnection Ressourcentyp
description: Statusinformationen über die Netzwerkverbindung im Zusammenhang mit der Benachrichtigung enthält.
ms.openlocfilehash: e3352cbda430412691285c209c566fb379045681
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019704"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="27fe2-103">NetworkConnection Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="27fe2-103">networkConnection resource type</span></span>

<span data-ttu-id="27fe2-104">Statusinformationen über die Netzwerkverbindung im Zusammenhang mit der Benachrichtigung enthält.</span><span class="sxs-lookup"><span data-stu-id="27fe2-104">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="27fe2-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="27fe2-105">Properties</span></span>

| <span data-ttu-id="27fe2-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="27fe2-106">Property</span></span>   | <span data-ttu-id="27fe2-107">Typ</span><span class="sxs-lookup"><span data-stu-id="27fe2-107">Type</span></span>|<span data-ttu-id="27fe2-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="27fe2-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27fe2-109">applicationName</span><span class="sxs-lookup"><span data-stu-id="27fe2-109">applicationName</span></span>|<span data-ttu-id="27fe2-110">String</span><span class="sxs-lookup"><span data-stu-id="27fe2-110">String</span></span>|<span data-ttu-id="27fe2-111">Name der Anwendung verwalten die Netzwerkschnittstelle (beispielsweise Facebook, SMTP, usw.).</span><span class="sxs-lookup"><span data-stu-id="27fe2-111">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="27fe2-112">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="27fe2-112">destinationAddress</span></span>|<span data-ttu-id="27fe2-113">String</span><span class="sxs-lookup"><span data-stu-id="27fe2-113">String</span></span>|<span data-ttu-id="27fe2-114">Ziel-IP-Adresse (der Verbindung).</span><span class="sxs-lookup"><span data-stu-id="27fe2-114">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="27fe2-115">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="27fe2-115">destinationDomain</span></span>|<span data-ttu-id="27fe2-116">String</span><span class="sxs-lookup"><span data-stu-id="27fe2-116">String</span></span>|<span data-ttu-id="27fe2-117">Ziel der Domänenteil der Ziel-URL.</span><span class="sxs-lookup"><span data-stu-id="27fe2-117">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="27fe2-118">(zum Beispiel "www.contoso.com").</span><span class="sxs-lookup"><span data-stu-id="27fe2-118">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="27fe2-119">destinationPort</span><span class="sxs-lookup"><span data-stu-id="27fe2-119">destinationPort</span></span>|<span data-ttu-id="27fe2-120">String</span><span class="sxs-lookup"><span data-stu-id="27fe2-120">String</span></span>|<span data-ttu-id="27fe2-121">Zielport (der Verbindung).</span><span class="sxs-lookup"><span data-stu-id="27fe2-121">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="27fe2-122">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="27fe2-122">destinationUrl</span></span>|<span data-ttu-id="27fe2-123">String</span><span class="sxs-lookup"><span data-stu-id="27fe2-123">String</span></span>|<span data-ttu-id="27fe2-124">Netzwerk-URL-URI-Verbindungszeichenfolge - Parameter ausschließen.</span><span class="sxs-lookup"><span data-stu-id="27fe2-124">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="27fe2-125">(zum Beispiel "www.contoso.com/products/default.html")</span><span class="sxs-lookup"><span data-stu-id="27fe2-125">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="27fe2-126">Richtung</span><span class="sxs-lookup"><span data-stu-id="27fe2-126">direction</span></span>|<span data-ttu-id="27fe2-127">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="27fe2-127">connectionDirection</span></span>|<span data-ttu-id="27fe2-128">Richtung der Netzwerk-Verbindung.</span><span class="sxs-lookup"><span data-stu-id="27fe2-128">Network connection direction.</span></span> <span data-ttu-id="27fe2-129">Mögliche Werte sind: `unknown`, `inbound` und `outbound`.</span><span class="sxs-lookup"><span data-stu-id="27fe2-129">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="27fe2-130">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="27fe2-130">domainRegisteredDateTime</span></span>|<span data-ttu-id="27fe2-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27fe2-131">DateTimeOffset</span></span>|<span data-ttu-id="27fe2-132">Datum, wenn die Zieldomäne registriert wurde.</span><span class="sxs-lookup"><span data-stu-id="27fe2-132">Date when the destination domain was registered.</span></span> <span data-ttu-id="27fe2-133">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="27fe2-133">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="27fe2-134">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="27fe2-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="27fe2-135">localDnsName</span><span class="sxs-lookup"><span data-stu-id="27fe2-135">localDnsName</span></span>|<span data-ttu-id="27fe2-136">String</span><span class="sxs-lookup"><span data-stu-id="27fe2-136">String</span></span>|<span data-ttu-id="27fe2-137">Der lokalen DNS-name Lösung, wie er in der Host lokalen DNS-Cache angezeigt wird (beispielsweise Fall, dass die Datei "Hosts" manipuliert wurde).</span><span class="sxs-lookup"><span data-stu-id="27fe2-137">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="27fe2-138">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="27fe2-138">natDestinationAddress</span></span>|<span data-ttu-id="27fe2-139">String</span><span class="sxs-lookup"><span data-stu-id="27fe2-139">String</span></span>|<span data-ttu-id="27fe2-140">Network Address Translation Ziel-IP-Adresse.</span><span class="sxs-lookup"><span data-stu-id="27fe2-140">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="27fe2-141">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="27fe2-141">natDestinationPort</span></span>|<span data-ttu-id="27fe2-142">String</span><span class="sxs-lookup"><span data-stu-id="27fe2-142">String</span></span>|<span data-ttu-id="27fe2-143">Network Address Translation Zielport.</span><span class="sxs-lookup"><span data-stu-id="27fe2-143">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="27fe2-144">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="27fe2-144">natSourceAddress</span></span>|<span data-ttu-id="27fe2-145">String</span><span class="sxs-lookup"><span data-stu-id="27fe2-145">String</span></span>|<span data-ttu-id="27fe2-146">Network Address Translation Quell-IP-Adresse.</span><span class="sxs-lookup"><span data-stu-id="27fe2-146">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="27fe2-147">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="27fe2-147">natSourcePort</span></span>|<span data-ttu-id="27fe2-148">String</span><span class="sxs-lookup"><span data-stu-id="27fe2-148">String</span></span>|<span data-ttu-id="27fe2-149">Network Address Translation Quellport.</span><span class="sxs-lookup"><span data-stu-id="27fe2-149">Network Address Translation source port.</span></span>|
|<span data-ttu-id="27fe2-150">protocol</span><span class="sxs-lookup"><span data-stu-id="27fe2-150">protocol</span></span>|[<span data-ttu-id="27fe2-151">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="27fe2-151">securityNetworkProtocol</span></span>](securitynetworkprotocol.md)|<span data-ttu-id="27fe2-152">Netzwerkprotokoll.</span><span class="sxs-lookup"><span data-stu-id="27fe2-152">Network protocol.</span></span> <span data-ttu-id="27fe2-153">Mögliche Werte sind: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd` , `raw`, `ipx`, `spx`, `spxII`.</span><span class="sxs-lookup"><span data-stu-id="27fe2-153">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="27fe2-154">riskScore</span><span class="sxs-lookup"><span data-stu-id="27fe2-154">riskScore</span></span>|<span data-ttu-id="27fe2-155">String</span><span class="sxs-lookup"><span data-stu-id="27fe2-155">String</span></span>|<span data-ttu-id="27fe2-156">Anbieter generiert/berechnet riskieren Bewertung der Verbindung.</span><span class="sxs-lookup"><span data-stu-id="27fe2-156">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="27fe2-157">Empfohlene Wertebereich von 0 bis 1, die den Prozentsatz entspricht.</span><span class="sxs-lookup"><span data-stu-id="27fe2-157">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="27fe2-158">sourceAddress</span><span class="sxs-lookup"><span data-stu-id="27fe2-158">sourceAddress</span></span>|<span data-ttu-id="27fe2-159">String</span><span class="sxs-lookup"><span data-stu-id="27fe2-159">String</span></span>|<span data-ttu-id="27fe2-160">Quelle (d. h. Ursprung) IP-Adresse (der Verbindung).</span><span class="sxs-lookup"><span data-stu-id="27fe2-160">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="27fe2-161">Quellport</span><span class="sxs-lookup"><span data-stu-id="27fe2-161">sourcePort</span></span>|<span data-ttu-id="27fe2-162">String</span><span class="sxs-lookup"><span data-stu-id="27fe2-162">String</span></span>|<span data-ttu-id="27fe2-163">Quelle (d. h. Ursprung) IP-Port (der Verbindung).</span><span class="sxs-lookup"><span data-stu-id="27fe2-163">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="27fe2-164">status</span><span class="sxs-lookup"><span data-stu-id="27fe2-164">status</span></span>|<span data-ttu-id="27fe2-165">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="27fe2-165">connectionStatus</span></span>|<span data-ttu-id="27fe2-166">Netzwerk-Verbindungsstatus.</span><span class="sxs-lookup"><span data-stu-id="27fe2-166">Network connection status.</span></span> <span data-ttu-id="27fe2-167">Mögliche Werte sind: `unknown`, `attempted`, `succeeded`, `blocked` und `failed`.</span><span class="sxs-lookup"><span data-stu-id="27fe2-167">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="27fe2-168">urlParameters</span><span class="sxs-lookup"><span data-stu-id="27fe2-168">urlParameters</span></span>|<span data-ttu-id="27fe2-169">String</span><span class="sxs-lookup"><span data-stu-id="27fe2-169">String</span></span>|<span data-ttu-id="27fe2-170">Parameter (Suffix) der Ziel-URL.</span><span class="sxs-lookup"><span data-stu-id="27fe2-170">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="27fe2-171">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="27fe2-171">JSON representation</span></span>

<span data-ttu-id="27fe2-172">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="27fe2-172">The following is a JSON representation of the resource.</span></span>

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