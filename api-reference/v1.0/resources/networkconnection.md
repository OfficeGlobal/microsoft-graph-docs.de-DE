---
title: NetworkConnection Ressourcentyp
description: Statusinformationen über die Netzwerkverbindung im Zusammenhang mit der Benachrichtigung enthält.
localization_priority: Normal
ms.openlocfilehash: 78ddcfd19d68b8dcd64c74a5beed6d1430f0ca38
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826509"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="edc43-103">NetworkConnection Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="edc43-103">networkConnection resource type</span></span>

<span data-ttu-id="edc43-104">Statusinformationen über die Netzwerkverbindung im Zusammenhang mit der Benachrichtigung enthält.</span><span class="sxs-lookup"><span data-stu-id="edc43-104">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="edc43-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="edc43-105">Properties</span></span>

| <span data-ttu-id="edc43-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="edc43-106">Property</span></span>   | <span data-ttu-id="edc43-107">Typ</span><span class="sxs-lookup"><span data-stu-id="edc43-107">Type</span></span>|<span data-ttu-id="edc43-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="edc43-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="edc43-109">applicationName</span><span class="sxs-lookup"><span data-stu-id="edc43-109">applicationName</span></span>|<span data-ttu-id="edc43-110">String</span><span class="sxs-lookup"><span data-stu-id="edc43-110">String</span></span>|<span data-ttu-id="edc43-111">Name der Anwendung verwalten die Netzwerkschnittstelle (beispielsweise Facebook, SMTP, usw.).</span><span class="sxs-lookup"><span data-stu-id="edc43-111">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="edc43-112">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="edc43-112">destinationAddress</span></span>|<span data-ttu-id="edc43-113">String</span><span class="sxs-lookup"><span data-stu-id="edc43-113">String</span></span>|<span data-ttu-id="edc43-114">Ziel-IP-Adresse (der Verbindung).</span><span class="sxs-lookup"><span data-stu-id="edc43-114">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="edc43-115">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="edc43-115">destinationDomain</span></span>|<span data-ttu-id="edc43-116">String</span><span class="sxs-lookup"><span data-stu-id="edc43-116">String</span></span>|<span data-ttu-id="edc43-117">Ziel der Domänenteil der Ziel-URL.</span><span class="sxs-lookup"><span data-stu-id="edc43-117">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="edc43-118">(zum Beispiel "www.contoso.com").</span><span class="sxs-lookup"><span data-stu-id="edc43-118">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="edc43-119">destinationPort</span><span class="sxs-lookup"><span data-stu-id="edc43-119">destinationPort</span></span>|<span data-ttu-id="edc43-120">String</span><span class="sxs-lookup"><span data-stu-id="edc43-120">String</span></span>|<span data-ttu-id="edc43-121">Zielport (der Verbindung).</span><span class="sxs-lookup"><span data-stu-id="edc43-121">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="edc43-122">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="edc43-122">destinationUrl</span></span>|<span data-ttu-id="edc43-123">String</span><span class="sxs-lookup"><span data-stu-id="edc43-123">String</span></span>|<span data-ttu-id="edc43-124">Netzwerk-URL-URI-Verbindungszeichenfolge - Parameter ausschließen.</span><span class="sxs-lookup"><span data-stu-id="edc43-124">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="edc43-125">(zum Beispiel "www.contoso.com/products/default.html")</span><span class="sxs-lookup"><span data-stu-id="edc43-125">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="edc43-126">Richtung</span><span class="sxs-lookup"><span data-stu-id="edc43-126">direction</span></span>|<span data-ttu-id="edc43-127">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="edc43-127">connectionDirection</span></span>|<span data-ttu-id="edc43-128">Richtung der Netzwerk-Verbindung.</span><span class="sxs-lookup"><span data-stu-id="edc43-128">Network connection direction.</span></span> <span data-ttu-id="edc43-129">Mögliche Werte sind: `unknown`, `inbound` und `outbound`.</span><span class="sxs-lookup"><span data-stu-id="edc43-129">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="edc43-130">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="edc43-130">domainRegisteredDateTime</span></span>|<span data-ttu-id="edc43-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edc43-131">DateTimeOffset</span></span>|<span data-ttu-id="edc43-132">Datum, wenn die Zieldomäne registriert wurde.</span><span class="sxs-lookup"><span data-stu-id="edc43-132">Date when the destination domain was registered.</span></span> <span data-ttu-id="edc43-133">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="edc43-133">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="edc43-134">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="edc43-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="edc43-135">localDnsName</span><span class="sxs-lookup"><span data-stu-id="edc43-135">localDnsName</span></span>|<span data-ttu-id="edc43-136">String</span><span class="sxs-lookup"><span data-stu-id="edc43-136">String</span></span>|<span data-ttu-id="edc43-137">Der lokalen DNS-name Lösung, wie er in der Host lokalen DNS-Cache angezeigt wird (beispielsweise Fall, dass die Datei "Hosts" manipuliert wurde).</span><span class="sxs-lookup"><span data-stu-id="edc43-137">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="edc43-138">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="edc43-138">natDestinationAddress</span></span>|<span data-ttu-id="edc43-139">String</span><span class="sxs-lookup"><span data-stu-id="edc43-139">String</span></span>|<span data-ttu-id="edc43-140">Network Address Translation Ziel-IP-Adresse.</span><span class="sxs-lookup"><span data-stu-id="edc43-140">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="edc43-141">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="edc43-141">natDestinationPort</span></span>|<span data-ttu-id="edc43-142">String</span><span class="sxs-lookup"><span data-stu-id="edc43-142">String</span></span>|<span data-ttu-id="edc43-143">Network Address Translation Zielport.</span><span class="sxs-lookup"><span data-stu-id="edc43-143">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="edc43-144">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="edc43-144">natSourceAddress</span></span>|<span data-ttu-id="edc43-145">String</span><span class="sxs-lookup"><span data-stu-id="edc43-145">String</span></span>|<span data-ttu-id="edc43-146">Network Address Translation Quell-IP-Adresse.</span><span class="sxs-lookup"><span data-stu-id="edc43-146">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="edc43-147">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="edc43-147">natSourcePort</span></span>|<span data-ttu-id="edc43-148">String</span><span class="sxs-lookup"><span data-stu-id="edc43-148">String</span></span>|<span data-ttu-id="edc43-149">Network Address Translation Quellport.</span><span class="sxs-lookup"><span data-stu-id="edc43-149">Network Address Translation source port.</span></span>|
|<span data-ttu-id="edc43-150">protocol</span><span class="sxs-lookup"><span data-stu-id="edc43-150">protocol</span></span>|[<span data-ttu-id="edc43-151">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="edc43-151">securityNetworkProtocol</span></span>](securitynetworkprotocol.md)|<span data-ttu-id="edc43-152">Netzwerkprotokoll.</span><span class="sxs-lookup"><span data-stu-id="edc43-152">Network protocol.</span></span> <span data-ttu-id="edc43-153">Mögliche Werte sind: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd` , `raw`, `ipx`, `spx`, `spxII`.</span><span class="sxs-lookup"><span data-stu-id="edc43-153">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="edc43-154">riskScore</span><span class="sxs-lookup"><span data-stu-id="edc43-154">riskScore</span></span>|<span data-ttu-id="edc43-155">String</span><span class="sxs-lookup"><span data-stu-id="edc43-155">String</span></span>|<span data-ttu-id="edc43-156">Anbieter generiert/berechnet riskieren Bewertung der Verbindung.</span><span class="sxs-lookup"><span data-stu-id="edc43-156">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="edc43-157">Empfohlene Wertebereich von 0 bis 1, die den Prozentsatz entspricht.</span><span class="sxs-lookup"><span data-stu-id="edc43-157">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="edc43-158">sourceAddress</span><span class="sxs-lookup"><span data-stu-id="edc43-158">sourceAddress</span></span>|<span data-ttu-id="edc43-159">String</span><span class="sxs-lookup"><span data-stu-id="edc43-159">String</span></span>|<span data-ttu-id="edc43-160">Quelle (d. h. Ursprung) IP-Adresse (der Verbindung).</span><span class="sxs-lookup"><span data-stu-id="edc43-160">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="edc43-161">Quellport</span><span class="sxs-lookup"><span data-stu-id="edc43-161">sourcePort</span></span>|<span data-ttu-id="edc43-162">String</span><span class="sxs-lookup"><span data-stu-id="edc43-162">String</span></span>|<span data-ttu-id="edc43-163">Quelle (d. h. Ursprung) IP-Port (der Verbindung).</span><span class="sxs-lookup"><span data-stu-id="edc43-163">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="edc43-164">status</span><span class="sxs-lookup"><span data-stu-id="edc43-164">status</span></span>|<span data-ttu-id="edc43-165">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="edc43-165">connectionStatus</span></span>|<span data-ttu-id="edc43-166">Netzwerk-Verbindungsstatus.</span><span class="sxs-lookup"><span data-stu-id="edc43-166">Network connection status.</span></span> <span data-ttu-id="edc43-167">Mögliche Werte sind: `unknown`, `attempted`, `succeeded`, `blocked` und `failed`.</span><span class="sxs-lookup"><span data-stu-id="edc43-167">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="edc43-168">urlParameters</span><span class="sxs-lookup"><span data-stu-id="edc43-168">urlParameters</span></span>|<span data-ttu-id="edc43-169">String</span><span class="sxs-lookup"><span data-stu-id="edc43-169">String</span></span>|<span data-ttu-id="edc43-170">Parameter (Suffix) der Ziel-URL.</span><span class="sxs-lookup"><span data-stu-id="edc43-170">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="edc43-171">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="edc43-171">JSON representation</span></span>

<span data-ttu-id="edc43-172">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="edc43-172">The following is a JSON representation of the resource.</span></span>

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
