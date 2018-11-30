---
title: Ressourcentyp hostSecurityState
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: ae64d4e0f13e39cb344fd54f5e600cfbfe0dc4f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061563"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="97ce2-104">Ressourcentyp hostSecurityState</span><span class="sxs-lookup"><span data-stu-id="97ce2-104">hostSecurityState resource type</span></span>

 > <span data-ttu-id="97ce2-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="97ce2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97ce2-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="97ce2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="97ce2-107">Enthält Statusinformationen über den Host (einschließlich der Geräte, Computer und usw.).</span><span class="sxs-lookup"><span data-stu-id="97ce2-107">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="97ce2-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="97ce2-108">Properties</span></span>

| <span data-ttu-id="97ce2-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="97ce2-109">Property</span></span>   | <span data-ttu-id="97ce2-110">Typ</span><span class="sxs-lookup"><span data-stu-id="97ce2-110">Type</span></span>|<span data-ttu-id="97ce2-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="97ce2-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97ce2-112">FQDN</span><span class="sxs-lookup"><span data-stu-id="97ce2-112">fqdn</span></span>|<span data-ttu-id="97ce2-113">String</span><span class="sxs-lookup"><span data-stu-id="97ce2-113">String</span></span>|<span data-ttu-id="97ce2-114">Host-FQDN (Fully Qualified Domain Name) (beispielsweise machine.company.com).</span><span class="sxs-lookup"><span data-stu-id="97ce2-114">Host FQDN (Fully Qualified Domain Name) (for example, machine.company.com).</span></span>|
|<span data-ttu-id="97ce2-115">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="97ce2-115">isAzureAadJoined</span></span>|<span data-ttu-id="97ce2-116">Boolesch</span><span class="sxs-lookup"><span data-stu-id="97ce2-116">Boolean</span></span>|<span data-ttu-id="97ce2-117">True, wenn der Host Domäne Azure Active Directory Domain Services beigetreten ist.</span><span class="sxs-lookup"><span data-stu-id="97ce2-117">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="97ce2-118">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="97ce2-118">isAzureAadRegistered</span></span>|<span data-ttu-id="97ce2-119">Boolesch</span><span class="sxs-lookup"><span data-stu-id="97ce2-119">Boolean</span></span>|<span data-ttu-id="97ce2-120">True, wenn der Host mit Azure Active Directory Gerät-Registrierung (BYOD Geräte - d. h., nicht vollständig durch Enterprise verwaltet) registriert.</span><span class="sxs-lookup"><span data-stu-id="97ce2-120">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="97ce2-121">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="97ce2-121">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="97ce2-122">Boolesch</span><span class="sxs-lookup"><span data-stu-id="97ce2-122">Boolean</span></span>|<span data-ttu-id="97ce2-123">True, wenn der Host der Domäne mit einer lokalen Active Directory-Domäne verbunden ist.</span><span class="sxs-lookup"><span data-stu-id="97ce2-123">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="97ce2-124">netBiosName</span><span class="sxs-lookup"><span data-stu-id="97ce2-124">netBiosName</span></span>|<span data-ttu-id="97ce2-125">String</span><span class="sxs-lookup"><span data-stu-id="97ce2-125">String</span></span>|<span data-ttu-id="97ce2-126">Der Name der lokalen Host ohne den DNS-Domänennamen.</span><span class="sxs-lookup"><span data-stu-id="97ce2-126">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="97ce2-127">Betriebssystem</span><span class="sxs-lookup"><span data-stu-id="97ce2-127">os</span></span>|<span data-ttu-id="97ce2-128">String</span><span class="sxs-lookup"><span data-stu-id="97ce2-128">String</span></span>|<span data-ttu-id="97ce2-129">Host-Betriebssystem.</span><span class="sxs-lookup"><span data-stu-id="97ce2-129">Host Operating System.</span></span> <span data-ttu-id="97ce2-130">(Z. B. Windows10, Mac OS, RHEL, usw.).</span><span class="sxs-lookup"><span data-stu-id="97ce2-130">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="97ce2-131">Priv.IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="97ce2-131">privateIpAddress</span></span>|<span data-ttu-id="97ce2-132">String</span><span class="sxs-lookup"><span data-stu-id="97ce2-132">String</span></span>|<span data-ttu-id="97ce2-133">Private (nicht-routingfähige) IPv4 oder IPv6-Adresse (siehe [RFC 1918](https://tools.ietf.org/html/rfc1918)) zum Zeitpunkt der Warnung.</span><span class="sxs-lookup"><span data-stu-id="97ce2-133">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="97ce2-134">Öffentl.IP</span><span class="sxs-lookup"><span data-stu-id="97ce2-134">publicIpAddress</span></span>|<span data-ttu-id="97ce2-135">String</span><span class="sxs-lookup"><span data-stu-id="97ce2-135">String</span></span>|<span data-ttu-id="97ce2-136">Öffentlich routingfähige IPv4 oder IPv6-Adresse (siehe [RFC 1918](https://tools.ietf.org/html/rfc1918)) zum Zeitpunkt der Warnung.</span><span class="sxs-lookup"><span data-stu-id="97ce2-136">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="97ce2-137">riskScore</span><span class="sxs-lookup"><span data-stu-id="97ce2-137">riskScore</span></span>|<span data-ttu-id="97ce2-138">String</span><span class="sxs-lookup"><span data-stu-id="97ce2-138">String</span></span>|<span data-ttu-id="97ce2-139">Provider-generiert/berechnet Risiko Bewertung des Hosts.</span><span class="sxs-lookup"><span data-stu-id="97ce2-139">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="97ce2-140">Empfohlene Wertebereich von 0 bis 1, die den Prozentsatz entspricht.</span><span class="sxs-lookup"><span data-stu-id="97ce2-140">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="97ce2-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="97ce2-141">JSON representation</span></span>

<span data-ttu-id="97ce2-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="97ce2-142">The following is a JSON representation of the resource.</span></span>

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
