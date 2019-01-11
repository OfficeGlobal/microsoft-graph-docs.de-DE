---
title: Ressourcentyp hostSecurityState
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: 1ae1436dd9771d34c37542eb756f81a4f8f0306a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853375"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="2eb64-104">Ressourcentyp hostSecurityState</span><span class="sxs-lookup"><span data-stu-id="2eb64-104">hostSecurityState resource type</span></span>

 > <span data-ttu-id="2eb64-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2eb64-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2eb64-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2eb64-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2eb64-107">Enthält Statusinformationen über den Host (einschließlich der Geräte, Computer und usw.).</span><span class="sxs-lookup"><span data-stu-id="2eb64-107">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="2eb64-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2eb64-108">Properties</span></span>

| <span data-ttu-id="2eb64-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2eb64-109">Property</span></span>   | <span data-ttu-id="2eb64-110">Typ</span><span class="sxs-lookup"><span data-stu-id="2eb64-110">Type</span></span>|<span data-ttu-id="2eb64-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2eb64-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2eb64-112">FQDN</span><span class="sxs-lookup"><span data-stu-id="2eb64-112">fqdn</span></span>|<span data-ttu-id="2eb64-113">String</span><span class="sxs-lookup"><span data-stu-id="2eb64-113">String</span></span>|<span data-ttu-id="2eb64-114">Host-FQDN (Fully Qualified Domain Name) (beispielsweise machine.company.com).</span><span class="sxs-lookup"><span data-stu-id="2eb64-114">Host FQDN (Fully Qualified Domain Name) (for example, machine.company.com).</span></span>|
|<span data-ttu-id="2eb64-115">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="2eb64-115">isAzureAadJoined</span></span>|<span data-ttu-id="2eb64-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="2eb64-116">Boolean</span></span>|<span data-ttu-id="2eb64-117">True, wenn der Host Domäne Azure Active Directory Domain Services beigetreten ist.</span><span class="sxs-lookup"><span data-stu-id="2eb64-117">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="2eb64-118">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="2eb64-118">isAzureAadRegistered</span></span>|<span data-ttu-id="2eb64-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="2eb64-119">Boolean</span></span>|<span data-ttu-id="2eb64-120">True, wenn der Host mit Azure Active Directory Gerät-Registrierung (BYOD Geräte - d. h., nicht vollständig durch Enterprise verwaltet) registriert.</span><span class="sxs-lookup"><span data-stu-id="2eb64-120">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="2eb64-121">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="2eb64-121">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="2eb64-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="2eb64-122">Boolean</span></span>|<span data-ttu-id="2eb64-123">True, wenn der Host der Domäne mit einer lokalen Active Directory-Domäne verbunden ist.</span><span class="sxs-lookup"><span data-stu-id="2eb64-123">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="2eb64-124">netBiosName</span><span class="sxs-lookup"><span data-stu-id="2eb64-124">netBiosName</span></span>|<span data-ttu-id="2eb64-125">String</span><span class="sxs-lookup"><span data-stu-id="2eb64-125">String</span></span>|<span data-ttu-id="2eb64-126">Der Name der lokalen Host ohne den DNS-Domänennamen.</span><span class="sxs-lookup"><span data-stu-id="2eb64-126">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="2eb64-127">Betriebssystem</span><span class="sxs-lookup"><span data-stu-id="2eb64-127">os</span></span>|<span data-ttu-id="2eb64-128">String</span><span class="sxs-lookup"><span data-stu-id="2eb64-128">String</span></span>|<span data-ttu-id="2eb64-129">Host-Betriebssystem.</span><span class="sxs-lookup"><span data-stu-id="2eb64-129">Host Operating System.</span></span> <span data-ttu-id="2eb64-130">(Z. B. Windows10, Mac OS, RHEL, usw.).</span><span class="sxs-lookup"><span data-stu-id="2eb64-130">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="2eb64-131">Priv.IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="2eb64-131">privateIpAddress</span></span>|<span data-ttu-id="2eb64-132">String</span><span class="sxs-lookup"><span data-stu-id="2eb64-132">String</span></span>|<span data-ttu-id="2eb64-133">Private (nicht-routingfähige) IPv4 oder IPv6-Adresse (siehe [RFC 1918](https://tools.ietf.org/html/rfc1918)) zum Zeitpunkt der Warnung.</span><span class="sxs-lookup"><span data-stu-id="2eb64-133">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="2eb64-134">Öffentl.IP</span><span class="sxs-lookup"><span data-stu-id="2eb64-134">publicIpAddress</span></span>|<span data-ttu-id="2eb64-135">String</span><span class="sxs-lookup"><span data-stu-id="2eb64-135">String</span></span>|<span data-ttu-id="2eb64-136">Öffentlich routingfähige IPv4 oder IPv6-Adresse (siehe [RFC 1918](https://tools.ietf.org/html/rfc1918)) zum Zeitpunkt der Warnung.</span><span class="sxs-lookup"><span data-stu-id="2eb64-136">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="2eb64-137">riskScore</span><span class="sxs-lookup"><span data-stu-id="2eb64-137">riskScore</span></span>|<span data-ttu-id="2eb64-138">String</span><span class="sxs-lookup"><span data-stu-id="2eb64-138">String</span></span>|<span data-ttu-id="2eb64-139">Provider-generiert/berechnet Risiko Bewertung des Hosts.</span><span class="sxs-lookup"><span data-stu-id="2eb64-139">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="2eb64-140">Empfohlene Wertebereich von 0 bis 1, die den Prozentsatz entspricht.</span><span class="sxs-lookup"><span data-stu-id="2eb64-140">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2eb64-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2eb64-141">JSON representation</span></span>

<span data-ttu-id="2eb64-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2eb64-142">The following is a JSON representation of the resource.</span></span>

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
