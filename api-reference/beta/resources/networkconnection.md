---
title: NetworkConnection Ressourcentyp
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: 6d28149854ed3157473b678db442ee3474e456c6
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571919"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="c7d79-104">NetworkConnection Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c7d79-104">networkConnection resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7d79-105">Statusinformationen über die Netzwerkverbindung im Zusammenhang mit der Benachrichtigung enthält.</span><span class="sxs-lookup"><span data-stu-id="c7d79-105">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="c7d79-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c7d79-106">Properties</span></span>

| <span data-ttu-id="c7d79-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c7d79-107">Property</span></span>   | <span data-ttu-id="c7d79-108">Typ</span><span class="sxs-lookup"><span data-stu-id="c7d79-108">Type</span></span>|<span data-ttu-id="c7d79-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c7d79-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7d79-110">applicationName</span><span class="sxs-lookup"><span data-stu-id="c7d79-110">applicationName</span></span>|<span data-ttu-id="c7d79-111">String</span><span class="sxs-lookup"><span data-stu-id="c7d79-111">String</span></span>|<span data-ttu-id="c7d79-112">Name der Anwendung verwalten die Netzwerkschnittstelle (beispielsweise Facebook, SMTP, usw.).</span><span class="sxs-lookup"><span data-stu-id="c7d79-112">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="c7d79-113">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="c7d79-113">destinationAddress</span></span>|<span data-ttu-id="c7d79-114">String</span><span class="sxs-lookup"><span data-stu-id="c7d79-114">String</span></span>|<span data-ttu-id="c7d79-115">Ziel-IP-Adresse (der Verbindung).</span><span class="sxs-lookup"><span data-stu-id="c7d79-115">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="c7d79-116">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="c7d79-116">destinationDomain</span></span>|<span data-ttu-id="c7d79-117">String</span><span class="sxs-lookup"><span data-stu-id="c7d79-117">String</span></span>|<span data-ttu-id="c7d79-118">Ziel der Domänenteil der Ziel-URL.</span><span class="sxs-lookup"><span data-stu-id="c7d79-118">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="c7d79-119">(zum Beispiel "www.contoso.com").</span><span class="sxs-lookup"><span data-stu-id="c7d79-119">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="c7d79-120">destinationPort</span><span class="sxs-lookup"><span data-stu-id="c7d79-120">destinationPort</span></span>|<span data-ttu-id="c7d79-121">String</span><span class="sxs-lookup"><span data-stu-id="c7d79-121">String</span></span>|<span data-ttu-id="c7d79-122">Zielport (der Verbindung).</span><span class="sxs-lookup"><span data-stu-id="c7d79-122">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="c7d79-123">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="c7d79-123">destinationUrl</span></span>|<span data-ttu-id="c7d79-124">String</span><span class="sxs-lookup"><span data-stu-id="c7d79-124">String</span></span>|<span data-ttu-id="c7d79-125">Netzwerk-URL-URI-Verbindungszeichenfolge - Parameter ausschließen.</span><span class="sxs-lookup"><span data-stu-id="c7d79-125">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="c7d79-126">(zum Beispiel "www.contoso.com/products/default.html")</span><span class="sxs-lookup"><span data-stu-id="c7d79-126">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="c7d79-127">Richtung</span><span class="sxs-lookup"><span data-stu-id="c7d79-127">direction</span></span>|<span data-ttu-id="c7d79-128">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="c7d79-128">connectionDirection</span></span>|<span data-ttu-id="c7d79-129">Richtung der Netzwerk-Verbindung.</span><span class="sxs-lookup"><span data-stu-id="c7d79-129">Network connection direction.</span></span> <span data-ttu-id="c7d79-130">Mögliche Werte sind: `unknown`, `inbound` und `outbound`.</span><span class="sxs-lookup"><span data-stu-id="c7d79-130">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="c7d79-131">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="c7d79-131">domainRegisteredDateTime</span></span>|<span data-ttu-id="c7d79-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7d79-132">DateTimeOffset</span></span>|<span data-ttu-id="c7d79-133">Datum, wenn die Zieldomäne registriert wurde.</span><span class="sxs-lookup"><span data-stu-id="c7d79-133">Date when the destination domain was registered.</span></span> <span data-ttu-id="c7d79-134">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="c7d79-134">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c7d79-135">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c7d79-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c7d79-136">localDnsName</span><span class="sxs-lookup"><span data-stu-id="c7d79-136">localDnsName</span></span>|<span data-ttu-id="c7d79-137">String</span><span class="sxs-lookup"><span data-stu-id="c7d79-137">String</span></span>|<span data-ttu-id="c7d79-138">Der lokalen DNS-name Lösung, wie er in der Host lokalen DNS-Cache angezeigt wird (beispielsweise Fall, dass die Datei "Hosts" manipuliert wurde).</span><span class="sxs-lookup"><span data-stu-id="c7d79-138">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="c7d79-139">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="c7d79-139">natDestinationAddress</span></span>|<span data-ttu-id="c7d79-140">String</span><span class="sxs-lookup"><span data-stu-id="c7d79-140">String</span></span>|<span data-ttu-id="c7d79-141">Network Address Translation Ziel-IP-Adresse.</span><span class="sxs-lookup"><span data-stu-id="c7d79-141">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="c7d79-142">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="c7d79-142">natDestinationPort</span></span>|<span data-ttu-id="c7d79-143">String</span><span class="sxs-lookup"><span data-stu-id="c7d79-143">String</span></span>|<span data-ttu-id="c7d79-144">Network Address Translation Zielport.</span><span class="sxs-lookup"><span data-stu-id="c7d79-144">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="c7d79-145">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="c7d79-145">natSourceAddress</span></span>|<span data-ttu-id="c7d79-146">String</span><span class="sxs-lookup"><span data-stu-id="c7d79-146">String</span></span>|<span data-ttu-id="c7d79-147">Network Address Translation Quell-IP-Adresse.</span><span class="sxs-lookup"><span data-stu-id="c7d79-147">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="c7d79-148">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="c7d79-148">natSourcePort</span></span>|<span data-ttu-id="c7d79-149">String</span><span class="sxs-lookup"><span data-stu-id="c7d79-149">String</span></span>|<span data-ttu-id="c7d79-150">Network Address Translation Quellport.</span><span class="sxs-lookup"><span data-stu-id="c7d79-150">Network Address Translation source port.</span></span>|
|<span data-ttu-id="c7d79-151">protocol</span><span class="sxs-lookup"><span data-stu-id="c7d79-151">protocol</span></span>| <span data-ttu-id="c7d79-152">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="c7d79-152">securityNetworkProtocol</span></span> |<span data-ttu-id="c7d79-153">Netzwerkprotokoll.</span><span class="sxs-lookup"><span data-stu-id="c7d79-153">Network protocol.</span></span> <span data-ttu-id="c7d79-154">Mögliche Werte sind: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd` , `raw`, `ipx`, `spx`, `spxII`.</span><span class="sxs-lookup"><span data-stu-id="c7d79-154">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="c7d79-155">riskScore</span><span class="sxs-lookup"><span data-stu-id="c7d79-155">riskScore</span></span>|<span data-ttu-id="c7d79-156">String</span><span class="sxs-lookup"><span data-stu-id="c7d79-156">String</span></span>|<span data-ttu-id="c7d79-157">Anbieter generiert/berechnet riskieren Bewertung der Verbindung.</span><span class="sxs-lookup"><span data-stu-id="c7d79-157">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="c7d79-158">Empfohlene Wertebereich von 0 bis 1, die den Prozentsatz entspricht.</span><span class="sxs-lookup"><span data-stu-id="c7d79-158">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="c7d79-159">sourceAddress</span><span class="sxs-lookup"><span data-stu-id="c7d79-159">sourceAddress</span></span>|<span data-ttu-id="c7d79-160">String</span><span class="sxs-lookup"><span data-stu-id="c7d79-160">String</span></span>|<span data-ttu-id="c7d79-161">Quelle (d. h. Ursprung) IP-Adresse (der Verbindung).</span><span class="sxs-lookup"><span data-stu-id="c7d79-161">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="c7d79-162">Quellport</span><span class="sxs-lookup"><span data-stu-id="c7d79-162">sourcePort</span></span>|<span data-ttu-id="c7d79-163">String</span><span class="sxs-lookup"><span data-stu-id="c7d79-163">String</span></span>|<span data-ttu-id="c7d79-164">Quelle (d. h. Ursprung) IP-Port (der Verbindung).</span><span class="sxs-lookup"><span data-stu-id="c7d79-164">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="c7d79-165">status</span><span class="sxs-lookup"><span data-stu-id="c7d79-165">status</span></span>|<span data-ttu-id="c7d79-166">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="c7d79-166">connectionStatus</span></span>|<span data-ttu-id="c7d79-167">Netzwerk-Verbindungsstatus.</span><span class="sxs-lookup"><span data-stu-id="c7d79-167">Network connection status.</span></span> <span data-ttu-id="c7d79-168">Mögliche Werte sind: `unknown`, `attempted`, `succeeded`, `blocked` und `failed`.</span><span class="sxs-lookup"><span data-stu-id="c7d79-168">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="c7d79-169">urlParameters</span><span class="sxs-lookup"><span data-stu-id="c7d79-169">urlParameters</span></span>|<span data-ttu-id="c7d79-170">String</span><span class="sxs-lookup"><span data-stu-id="c7d79-170">String</span></span>|<span data-ttu-id="c7d79-171">Parameter (Suffix) der Ziel-URL.</span><span class="sxs-lookup"><span data-stu-id="c7d79-171">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c7d79-172">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c7d79-172">JSON representation</span></span>

<span data-ttu-id="c7d79-173">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c7d79-173">The following is a JSON representation of the resource.</span></span>

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
