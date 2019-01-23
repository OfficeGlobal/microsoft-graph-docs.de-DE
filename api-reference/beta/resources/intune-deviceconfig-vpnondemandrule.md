---
title: Ressourcentyp vpnOnDemandRule
description: VPN-On-Demand Regeldefinition.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8164d1c12aeb172120bb9803d7f3dd98366ec948
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421459"
---
# <a name="vpnondemandrule-resource-type"></a><span data-ttu-id="10dc9-103">Ressourcentyp vpnOnDemandRule</span><span class="sxs-lookup"><span data-stu-id="10dc9-103">vpnOnDemandRule resource type</span></span>

> <span data-ttu-id="10dc9-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="10dc9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="10dc9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="10dc9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="10dc9-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="10dc9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10dc9-107">VPN-On-Demand Regeldefinition.</span><span class="sxs-lookup"><span data-stu-id="10dc9-107">VPN On-Demand Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="10dc9-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="10dc9-108">Properties</span></span>
|<span data-ttu-id="10dc9-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="10dc9-109">Property</span></span>|<span data-ttu-id="10dc9-110">Typ</span><span class="sxs-lookup"><span data-stu-id="10dc9-110">Type</span></span>|<span data-ttu-id="10dc9-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="10dc9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10dc9-112">SSIDs</span><span class="sxs-lookup"><span data-stu-id="10dc9-112">ssids</span></span>|<span data-ttu-id="10dc9-113">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="10dc9-113">String collection</span></span>|<span data-ttu-id="10dc9-114">Netzwerkdienst festgelegt (SSIDs Identifiers).</span><span class="sxs-lookup"><span data-stu-id="10dc9-114">Network Service Set Identifiers (SSIDs).</span></span>|
|<span data-ttu-id="10dc9-115">dnsSearchDomains</span><span class="sxs-lookup"><span data-stu-id="10dc9-115">dnsSearchDomains</span></span>|<span data-ttu-id="10dc9-116">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="10dc9-116">String collection</span></span>|<span data-ttu-id="10dc9-117">DNS-Suche Domänen.</span><span class="sxs-lookup"><span data-stu-id="10dc9-117">DNS Search Domains.</span></span>|
|<span data-ttu-id="10dc9-118">probeUrl</span><span class="sxs-lookup"><span data-stu-id="10dc9-118">probeUrl</span></span>|<span data-ttu-id="10dc9-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="10dc9-119">String</span></span>|<span data-ttu-id="10dc9-120">Eine URL zu belegen.</span><span class="sxs-lookup"><span data-stu-id="10dc9-120">A URL to probe.</span></span> <span data-ttu-id="10dc9-121">Wenn diese URL erfolgreich ist ohne Umleitung abgerufen (einen 200 HTTP-Statuscode zurückgibt), die dieser Regel entspricht.</span><span class="sxs-lookup"><span data-stu-id="10dc9-121">If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.</span></span>|
|<span data-ttu-id="10dc9-122">Aktion</span><span class="sxs-lookup"><span data-stu-id="10dc9-122">action</span></span>|[<span data-ttu-id="10dc9-123">vpnOnDemandRuleConnectionAction</span><span class="sxs-lookup"><span data-stu-id="10dc9-123">vpnOnDemandRuleConnectionAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|<span data-ttu-id="10dc9-124">Aktion.</span><span class="sxs-lookup"><span data-stu-id="10dc9-124">Action.</span></span> <span data-ttu-id="10dc9-125">Mögliche Werte: sind `connect`, `evaluateConnection`, `ignore` und `disconnect`.</span><span class="sxs-lookup"><span data-stu-id="10dc9-125">Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span></span>|
|<span data-ttu-id="10dc9-126">domainAction</span><span class="sxs-lookup"><span data-stu-id="10dc9-126">domainAction</span></span>|[<span data-ttu-id="10dc9-127">vpnOnDemandRuleConnectionDomainAction</span><span class="sxs-lookup"><span data-stu-id="10dc9-127">vpnOnDemandRuleConnectionDomainAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|<span data-ttu-id="10dc9-128">Domäne-Aktion (gilt nur bei der Aktion Verbindung bewerten ist).</span><span class="sxs-lookup"><span data-stu-id="10dc9-128">Domain Action (Only applicable when Action is evaluate connection).</span></span> <span data-ttu-id="10dc9-129">Mögliche Werte sind: `connectIfNeeded` und `neverConnect`.</span><span class="sxs-lookup"><span data-stu-id="10dc9-129">Possible values are: `connectIfNeeded`, `neverConnect`.</span></span>|
|<span data-ttu-id="10dc9-130">Domänen</span><span class="sxs-lookup"><span data-stu-id="10dc9-130">domains</span></span>|<span data-ttu-id="10dc9-131">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="10dc9-131">String collection</span></span>|<span data-ttu-id="10dc9-132">Domänen (gilt nur bei der Aktion Verbindung bewerten ist).</span><span class="sxs-lookup"><span data-stu-id="10dc9-132">Domains (Only applicable when Action is evaluate connection).</span></span>|
|<span data-ttu-id="10dc9-133">probeRequiredUrl</span><span class="sxs-lookup"><span data-stu-id="10dc9-133">probeRequiredUrl</span></span>|<span data-ttu-id="10dc9-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="10dc9-134">String</span></span>|<span data-ttu-id="10dc9-135">Prüfpunkt erforderliche Url (gilt nur bei der Aktion wird Verbindung bewerten und DomainAction ist eine Verbindung herstellen, falls erforderlich).</span><span class="sxs-lookup"><span data-stu-id="10dc9-135">Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).</span></span>|

## <a name="relationships"></a><span data-ttu-id="10dc9-136">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="10dc9-136">Relationships</span></span>
<span data-ttu-id="10dc9-137">Keine</span><span class="sxs-lookup"><span data-stu-id="10dc9-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="10dc9-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="10dc9-138">JSON Representation</span></span>
<span data-ttu-id="10dc9-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="10dc9-139">Here is a JSON representation of the resource.</span></span>
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




