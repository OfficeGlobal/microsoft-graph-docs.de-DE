---
title: Ressourcentyp hostSecurityState
description: Enthält Statusinformationen über den Host (einschließlich der Geräte, Computer und usw.).
localization_priority: Normal
ms.openlocfilehash: 0646547b7f3e31dcf283c1ce423a52b4ae16f013
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816338"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="85b65-103">Ressourcentyp hostSecurityState</span><span class="sxs-lookup"><span data-stu-id="85b65-103">hostSecurityState resource type</span></span>

<span data-ttu-id="85b65-104">Enthält Statusinformationen über den Host (einschließlich der Geräte, Computer und usw.).</span><span class="sxs-lookup"><span data-stu-id="85b65-104">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="85b65-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="85b65-105">Properties</span></span>

| <span data-ttu-id="85b65-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="85b65-106">Property</span></span>   | <span data-ttu-id="85b65-107">Typ</span><span class="sxs-lookup"><span data-stu-id="85b65-107">Type</span></span>|<span data-ttu-id="85b65-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="85b65-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85b65-109">FQDN</span><span class="sxs-lookup"><span data-stu-id="85b65-109">fqdn</span></span>|<span data-ttu-id="85b65-110">String</span><span class="sxs-lookup"><span data-stu-id="85b65-110">String</span></span>|<span data-ttu-id="85b65-111">Hosten der FQDN (Fully Qualified Domain Name) (z. B. `machine.company.com`).</span><span class="sxs-lookup"><span data-stu-id="85b65-111">Host FQDN (Fully Qualified Domain Name) (for example, `machine.company.com`).</span></span>|
|<span data-ttu-id="85b65-112">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="85b65-112">isAzureAadJoined</span></span>|<span data-ttu-id="85b65-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="85b65-113">Boolean</span></span>|<span data-ttu-id="85b65-114">True, wenn der Host Domäne Azure Active Directory Domain Services beigetreten ist.</span><span class="sxs-lookup"><span data-stu-id="85b65-114">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="85b65-115">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="85b65-115">isAzureAadRegistered</span></span>|<span data-ttu-id="85b65-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="85b65-116">Boolean</span></span>|<span data-ttu-id="85b65-117">True, wenn der Host mit Azure Active Directory Gerät-Registrierung (BYOD Geräte - d. h., nicht vollständig durch Enterprise verwaltet) registriert.</span><span class="sxs-lookup"><span data-stu-id="85b65-117">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="85b65-118">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="85b65-118">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="85b65-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="85b65-119">Boolean</span></span>|<span data-ttu-id="85b65-120">True, wenn der Host der Domäne mit einer lokalen Active Directory-Domäne verbunden ist.</span><span class="sxs-lookup"><span data-stu-id="85b65-120">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="85b65-121">netBiosName</span><span class="sxs-lookup"><span data-stu-id="85b65-121">netBiosName</span></span>|<span data-ttu-id="85b65-122">String</span><span class="sxs-lookup"><span data-stu-id="85b65-122">String</span></span>|<span data-ttu-id="85b65-123">Der Name der lokalen Host ohne den DNS-Domänennamen.</span><span class="sxs-lookup"><span data-stu-id="85b65-123">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="85b65-124">Betriebssystem</span><span class="sxs-lookup"><span data-stu-id="85b65-124">os</span></span>|<span data-ttu-id="85b65-125">String</span><span class="sxs-lookup"><span data-stu-id="85b65-125">String</span></span>|<span data-ttu-id="85b65-126">Host-Betriebssystem.</span><span class="sxs-lookup"><span data-stu-id="85b65-126">Host Operating System.</span></span> <span data-ttu-id="85b65-127">(Z. B. Windows10, Mac OS, RHEL, usw.).</span><span class="sxs-lookup"><span data-stu-id="85b65-127">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="85b65-128">Priv.IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="85b65-128">privateIpAddress</span></span>|<span data-ttu-id="85b65-129">String</span><span class="sxs-lookup"><span data-stu-id="85b65-129">String</span></span>|<span data-ttu-id="85b65-130">Private (nicht-routingfähige) IPv4 oder IPv6-Adresse (siehe [RFC 1918](https://tools.ietf.org/html/rfc1918)) zum Zeitpunkt der Warnung.</span><span class="sxs-lookup"><span data-stu-id="85b65-130">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="85b65-131">Öffentl.IP</span><span class="sxs-lookup"><span data-stu-id="85b65-131">publicIpAddress</span></span>|<span data-ttu-id="85b65-132">String</span><span class="sxs-lookup"><span data-stu-id="85b65-132">String</span></span>|<span data-ttu-id="85b65-133">Öffentlich routingfähige IPv4 oder IPv6-Adresse (siehe [RFC 1918](https://tools.ietf.org/html/rfc1918)) zum Zeitpunkt der Warnung.</span><span class="sxs-lookup"><span data-stu-id="85b65-133">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="85b65-134">riskScore</span><span class="sxs-lookup"><span data-stu-id="85b65-134">riskScore</span></span>|<span data-ttu-id="85b65-135">String</span><span class="sxs-lookup"><span data-stu-id="85b65-135">String</span></span>|<span data-ttu-id="85b65-136">Provider-generiert/berechnet Risiko Bewertung des Hosts.</span><span class="sxs-lookup"><span data-stu-id="85b65-136">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="85b65-137">Empfohlene Wertebereich von 0 bis 1, die den Prozentsatz entspricht.</span><span class="sxs-lookup"><span data-stu-id="85b65-137">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="85b65-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="85b65-138">JSON representation</span></span>

<span data-ttu-id="85b65-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="85b65-139">The following is a JSON representation of the resource.</span></span>

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
