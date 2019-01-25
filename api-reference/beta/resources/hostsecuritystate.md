---
title: Ressourcentyp hostSecurityState
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: d6f566a2bd42163c570fe837d2419057c62664bb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526697"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="64e29-104">Ressourcentyp hostSecurityState</span><span class="sxs-lookup"><span data-stu-id="64e29-104">hostSecurityState resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64e29-105">Enthält Statusinformationen über den Host (einschließlich der Geräte, Computer und usw.).</span><span class="sxs-lookup"><span data-stu-id="64e29-105">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="64e29-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="64e29-106">Properties</span></span>

| <span data-ttu-id="64e29-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="64e29-107">Property</span></span>   | <span data-ttu-id="64e29-108">Typ</span><span class="sxs-lookup"><span data-stu-id="64e29-108">Type</span></span>|<span data-ttu-id="64e29-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="64e29-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="64e29-110">FQDN</span><span class="sxs-lookup"><span data-stu-id="64e29-110">fqdn</span></span>|<span data-ttu-id="64e29-111">String</span><span class="sxs-lookup"><span data-stu-id="64e29-111">String</span></span>|<span data-ttu-id="64e29-112">Host-FQDN (Fully Qualified Domain Name) (beispielsweise machine.company.com).</span><span class="sxs-lookup"><span data-stu-id="64e29-112">Host FQDN (Fully Qualified Domain Name) (for example, machine.company.com).</span></span>|
|<span data-ttu-id="64e29-113">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="64e29-113">isAzureAadJoined</span></span>|<span data-ttu-id="64e29-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="64e29-114">Boolean</span></span>|<span data-ttu-id="64e29-115">True, wenn der Host Domäne Azure Active Directory Domain Services beigetreten ist.</span><span class="sxs-lookup"><span data-stu-id="64e29-115">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="64e29-116">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="64e29-116">isAzureAadRegistered</span></span>|<span data-ttu-id="64e29-117">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="64e29-117">Boolean</span></span>|<span data-ttu-id="64e29-118">True, wenn der Host mit Azure Active Directory Gerät-Registrierung (BYOD Geräte - d. h., nicht vollständig durch Enterprise verwaltet) registriert.</span><span class="sxs-lookup"><span data-stu-id="64e29-118">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="64e29-119">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="64e29-119">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="64e29-120">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="64e29-120">Boolean</span></span>|<span data-ttu-id="64e29-121">True, wenn der Host der Domäne mit einer lokalen Active Directory-Domäne verbunden ist.</span><span class="sxs-lookup"><span data-stu-id="64e29-121">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="64e29-122">netBiosName</span><span class="sxs-lookup"><span data-stu-id="64e29-122">netBiosName</span></span>|<span data-ttu-id="64e29-123">String</span><span class="sxs-lookup"><span data-stu-id="64e29-123">String</span></span>|<span data-ttu-id="64e29-124">Der Name der lokalen Host ohne den DNS-Domänennamen.</span><span class="sxs-lookup"><span data-stu-id="64e29-124">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="64e29-125">I-5.</span><span class="sxs-lookup"><span data-stu-id="64e29-125">os</span></span>|<span data-ttu-id="64e29-126">String</span><span class="sxs-lookup"><span data-stu-id="64e29-126">String</span></span>|<span data-ttu-id="64e29-127">Host-Betriebssystem.</span><span class="sxs-lookup"><span data-stu-id="64e29-127">Host Operating System.</span></span> <span data-ttu-id="64e29-128">(Z. B. Windows10, Mac OS, RHEL, usw.).</span><span class="sxs-lookup"><span data-stu-id="64e29-128">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="64e29-129">Priv.IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="64e29-129">privateIpAddress</span></span>|<span data-ttu-id="64e29-130">String</span><span class="sxs-lookup"><span data-stu-id="64e29-130">String</span></span>|<span data-ttu-id="64e29-131">Private (nicht-routingfähige) IPv4 oder IPv6-Adresse (siehe [RFC 1918](https://tools.ietf.org/html/rfc1918)) zum Zeitpunkt der Warnung.</span><span class="sxs-lookup"><span data-stu-id="64e29-131">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="64e29-132">Öffentl.IP</span><span class="sxs-lookup"><span data-stu-id="64e29-132">publicIpAddress</span></span>|<span data-ttu-id="64e29-133">String</span><span class="sxs-lookup"><span data-stu-id="64e29-133">String</span></span>|<span data-ttu-id="64e29-134">Öffentlich routingfähige IPv4 oder IPv6-Adresse (siehe [RFC 1918](https://tools.ietf.org/html/rfc1918)) zum Zeitpunkt der Warnung.</span><span class="sxs-lookup"><span data-stu-id="64e29-134">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="64e29-135">riskScore</span><span class="sxs-lookup"><span data-stu-id="64e29-135">riskScore</span></span>|<span data-ttu-id="64e29-136">String</span><span class="sxs-lookup"><span data-stu-id="64e29-136">String</span></span>|<span data-ttu-id="64e29-137">Provider-generiert/berechnet Risiko Bewertung des Hosts.</span><span class="sxs-lookup"><span data-stu-id="64e29-137">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="64e29-138">Empfohlene Wertebereich von 0 bis 1, die den Prozentsatz entspricht.</span><span class="sxs-lookup"><span data-stu-id="64e29-138">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="64e29-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="64e29-139">JSON representation</span></span>

<span data-ttu-id="64e29-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="64e29-140">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "hostSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/hostsecuritystate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
