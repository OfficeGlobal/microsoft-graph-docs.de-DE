---
title: Ressourcentyp vpnOnDemandRule
description: VPN-On-Demand Regeldefinition.
author: tfitzmac
ms.openlocfilehash: 72b85971dc9c613026bb9e720ca55165845e0c9e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352192"
---
# <a name="vpnondemandrule-resource-type"></a><span data-ttu-id="7b397-103">Ressourcentyp vpnOnDemandRule</span><span class="sxs-lookup"><span data-stu-id="7b397-103">vpnOnDemandRule resource type</span></span>

> <span data-ttu-id="7b397-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7b397-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b397-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7b397-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7b397-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7b397-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7b397-107">VPN-On-Demand Regeldefinition.</span><span class="sxs-lookup"><span data-stu-id="7b397-107">VPN On-Demand Rule definition.</span></span>
## <a name="properties"></a><span data-ttu-id="7b397-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7b397-108">Properties</span></span>
|<span data-ttu-id="7b397-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7b397-109">Property</span></span>|<span data-ttu-id="7b397-110">Typ</span><span class="sxs-lookup"><span data-stu-id="7b397-110">Type</span></span>|<span data-ttu-id="7b397-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7b397-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b397-112">SSIDs</span><span class="sxs-lookup"><span data-stu-id="7b397-112">ssids</span></span>|<span data-ttu-id="7b397-113">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="7b397-113">String collection</span></span>|<span data-ttu-id="7b397-114">Netzwerkdienst festgelegt (SSIDs Identifiers).</span><span class="sxs-lookup"><span data-stu-id="7b397-114">Network Service Set Identifiers (SSIDs).</span></span>|
|<span data-ttu-id="7b397-115">dnsSearchDomains</span><span class="sxs-lookup"><span data-stu-id="7b397-115">dnsSearchDomains</span></span>|<span data-ttu-id="7b397-116">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="7b397-116">String collection</span></span>|<span data-ttu-id="7b397-117">DNS-Suche Domänen.</span><span class="sxs-lookup"><span data-stu-id="7b397-117">DNS Search Domains.</span></span>|
|<span data-ttu-id="7b397-118">probeUrl</span><span class="sxs-lookup"><span data-stu-id="7b397-118">probeUrl</span></span>|<span data-ttu-id="7b397-119">String</span><span class="sxs-lookup"><span data-stu-id="7b397-119">String</span></span>|<span data-ttu-id="7b397-120">Eine URL zu belegen.</span><span class="sxs-lookup"><span data-stu-id="7b397-120">A URL to probe.</span></span> <span data-ttu-id="7b397-121">Wenn diese URL erfolgreich ist ohne Umleitung abgerufen (einen 200 HTTP-Statuscode zurückgibt), die dieser Regel entspricht.</span><span class="sxs-lookup"><span data-stu-id="7b397-121">If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.</span></span>|
|<span data-ttu-id="7b397-122">Aktion</span><span class="sxs-lookup"><span data-stu-id="7b397-122">action</span></span>|[<span data-ttu-id="7b397-123">vpnOnDemandRuleConnectionAction</span><span class="sxs-lookup"><span data-stu-id="7b397-123">vpnOnDemandRuleConnectionAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|<span data-ttu-id="7b397-124">Aktion.</span><span class="sxs-lookup"><span data-stu-id="7b397-124">Action.</span></span> <span data-ttu-id="7b397-125">Mögliche Werte: sind `connect`, `evaluateConnection`, `ignore` und `disconnect`.</span><span class="sxs-lookup"><span data-stu-id="7b397-125">Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span></span>|
|<span data-ttu-id="7b397-126">domainAction</span><span class="sxs-lookup"><span data-stu-id="7b397-126">domainAction</span></span>|[<span data-ttu-id="7b397-127">vpnOnDemandRuleConnectionDomainAction</span><span class="sxs-lookup"><span data-stu-id="7b397-127">vpnOnDemandRuleConnectionDomainAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|<span data-ttu-id="7b397-128">Domäne-Aktion (gilt nur bei der Aktion Verbindung bewerten ist).</span><span class="sxs-lookup"><span data-stu-id="7b397-128">Domain Action (Only applicable when Action is evaluate connection).</span></span> <span data-ttu-id="7b397-129">Mögliche Werte sind: `connectIfNeeded` und `neverConnect`.</span><span class="sxs-lookup"><span data-stu-id="7b397-129">Possible values are: `connectIfNeeded`, `neverConnect`.</span></span>|
|<span data-ttu-id="7b397-130">Domänen</span><span class="sxs-lookup"><span data-stu-id="7b397-130">domains</span></span>|<span data-ttu-id="7b397-131">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="7b397-131">String collection</span></span>|<span data-ttu-id="7b397-132">Domänen (gilt nur bei der Aktion Verbindung bewerten ist).</span><span class="sxs-lookup"><span data-stu-id="7b397-132">Domains (Only applicable when Action is evaluate connection).</span></span>|
|<span data-ttu-id="7b397-133">probeRequiredUrl</span><span class="sxs-lookup"><span data-stu-id="7b397-133">probeRequiredUrl</span></span>|<span data-ttu-id="7b397-134">String</span><span class="sxs-lookup"><span data-stu-id="7b397-134">String</span></span>|<span data-ttu-id="7b397-135">Prüfpunkt erforderliche Url (gilt nur bei der Aktion wird Verbindung bewerten und DomainAction ist eine Verbindung herstellen, falls erforderlich).</span><span class="sxs-lookup"><span data-stu-id="7b397-135">Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b397-136">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7b397-136">Relationships</span></span>
<span data-ttu-id="7b397-137">Keine</span><span class="sxs-lookup"><span data-stu-id="7b397-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7b397-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7b397-138">JSON Representation</span></span>
<span data-ttu-id="7b397-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7b397-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnOnDemandRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnOnDemandRule",
  "ssids": [
    "String"
  ],
  "dnsSearchDomains": [
    "String"
  ],
  "probeUrl": "String",
  "action": "String",
  "domainAction": "String",
  "domains": [
    "String"
  ],
  "probeRequiredUrl": "String"
}
```





