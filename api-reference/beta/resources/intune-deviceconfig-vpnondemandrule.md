---
title: vpnOnDemandRule-Ressourcentyp
description: Definition der VPN-on-Demand-Regel.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b1bccd015e45291b344e7c77df4ac5c0a0af07d0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161586"
---
# <a name="vpnondemandrule-resource-type"></a><span data-ttu-id="9cadd-103">vpnOnDemandRule-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9cadd-103">vpnOnDemandRule resource type</span></span>

> <span data-ttu-id="9cadd-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9cadd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9cadd-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9cadd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cadd-106">Definition der VPN-on-Demand-Regel.</span><span class="sxs-lookup"><span data-stu-id="9cadd-106">VPN On-Demand Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="9cadd-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9cadd-107">Properties</span></span>
|<span data-ttu-id="9cadd-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9cadd-108">Property</span></span>|<span data-ttu-id="9cadd-109">Typ</span><span class="sxs-lookup"><span data-stu-id="9cadd-109">Type</span></span>|<span data-ttu-id="9cadd-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9cadd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cadd-111">SSIDs</span><span class="sxs-lookup"><span data-stu-id="9cadd-111">ssids</span></span>|<span data-ttu-id="9cadd-112">String collection</span><span class="sxs-lookup"><span data-stu-id="9cadd-112">String collection</span></span>|<span data-ttu-id="9cadd-113">Netzwerkdienst Satz-IDs (SSIDs).</span><span class="sxs-lookup"><span data-stu-id="9cadd-113">Network Service Set Identifiers (SSIDs).</span></span>|
|<span data-ttu-id="9cadd-114">dnsSearchDomains</span><span class="sxs-lookup"><span data-stu-id="9cadd-114">dnsSearchDomains</span></span>|<span data-ttu-id="9cadd-115">String collection</span><span class="sxs-lookup"><span data-stu-id="9cadd-115">String collection</span></span>|<span data-ttu-id="9cadd-116">DNS-Such Domänen.</span><span class="sxs-lookup"><span data-stu-id="9cadd-116">DNS Search Domains.</span></span>|
|<span data-ttu-id="9cadd-117">probeUrl</span><span class="sxs-lookup"><span data-stu-id="9cadd-117">probeUrl</span></span>|<span data-ttu-id="9cadd-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9cadd-118">String</span></span>|<span data-ttu-id="9cadd-119">Eine zu über URL.</span><span class="sxs-lookup"><span data-stu-id="9cadd-119">A URL to probe.</span></span> <span data-ttu-id="9cadd-120">Wenn diese URL erfolgreich abgerufen wird (zurückgeben eines 200 HTTP-Statuscodes) ohne Umleitung, stimmt diese Regel überein.</span><span class="sxs-lookup"><span data-stu-id="9cadd-120">If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.</span></span>|
|<span data-ttu-id="9cadd-121">Aktion</span><span class="sxs-lookup"><span data-stu-id="9cadd-121">action</span></span>|[<span data-ttu-id="9cadd-122">vpnOnDemandRuleConnectionAction</span><span class="sxs-lookup"><span data-stu-id="9cadd-122">vpnOnDemandRuleConnectionAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|<span data-ttu-id="9cadd-123">Aktion.</span><span class="sxs-lookup"><span data-stu-id="9cadd-123">Action.</span></span> <span data-ttu-id="9cadd-124">Mögliche Werte: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span><span class="sxs-lookup"><span data-stu-id="9cadd-124">Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span></span>|
|<span data-ttu-id="9cadd-125">Domäne</span><span class="sxs-lookup"><span data-stu-id="9cadd-125">domainAction</span></span>|[<span data-ttu-id="9cadd-126">vpnOnDemandRuleConnectionDomainAction</span><span class="sxs-lookup"><span data-stu-id="9cadd-126">vpnOnDemandRuleConnectionDomainAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|<span data-ttu-id="9cadd-127">Domänen Aktion (gilt nur, wenn die Aktion die Verbindung auswertet).</span><span class="sxs-lookup"><span data-stu-id="9cadd-127">Domain Action (Only applicable when Action is evaluate connection).</span></span> <span data-ttu-id="9cadd-128">Mögliche Werte sind: `connectIfNeeded` und `neverConnect`.</span><span class="sxs-lookup"><span data-stu-id="9cadd-128">Possible values are: `connectIfNeeded`, `neverConnect`.</span></span>|
|<span data-ttu-id="9cadd-129">Domänen</span><span class="sxs-lookup"><span data-stu-id="9cadd-129">domains</span></span>|<span data-ttu-id="9cadd-130">String collection</span><span class="sxs-lookup"><span data-stu-id="9cadd-130">String collection</span></span>|<span data-ttu-id="9cadd-131">Domänen (gilt nur, wenn die Aktion die Verbindung auswertet).</span><span class="sxs-lookup"><span data-stu-id="9cadd-131">Domains (Only applicable when Action is evaluate connection).</span></span>|
|<span data-ttu-id="9cadd-132">probeRequiredUrl</span><span class="sxs-lookup"><span data-stu-id="9cadd-132">probeRequiredUrl</span></span>|<span data-ttu-id="9cadd-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9cadd-133">String</span></span>|<span data-ttu-id="9cadd-134">Überprüfen Sie die erforderliche URL (gilt nur, wenn die Aktion die Verbindung auswertet und wenn erforderlich die Domäne "Connect" ist).</span><span class="sxs-lookup"><span data-stu-id="9cadd-134">Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).</span></span>|

## <a name="relationships"></a><span data-ttu-id="9cadd-135">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9cadd-135">Relationships</span></span>
<span data-ttu-id="9cadd-136">Keine</span><span class="sxs-lookup"><span data-stu-id="9cadd-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9cadd-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9cadd-137">JSON Representation</span></span>
<span data-ttu-id="9cadd-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9cadd-138">Here is a JSON representation of the resource.</span></span>
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




