---
title: vpnDnsRule-Ressourcentyp
description: Definition der VPN-DNS-Regel.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 545c0dd8a84f19888452261e350a9b347061595c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158506"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="0db0b-103">vpnDnsRule-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0db0b-103">vpnDnsRule resource type</span></span>

> <span data-ttu-id="0db0b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0db0b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0db0b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0db0b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0db0b-106">Definition der VPN-DNS-Regel.</span><span class="sxs-lookup"><span data-stu-id="0db0b-106">VPN DNS Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="0db0b-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0db0b-107">Properties</span></span>
|<span data-ttu-id="0db0b-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0db0b-108">Property</span></span>|<span data-ttu-id="0db0b-109">Typ</span><span class="sxs-lookup"><span data-stu-id="0db0b-109">Type</span></span>|<span data-ttu-id="0db0b-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0db0b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0db0b-111">name</span><span class="sxs-lookup"><span data-stu-id="0db0b-111">name</span></span>|<span data-ttu-id="0db0b-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0db0b-112">String</span></span>|<span data-ttu-id="0db0b-113">Namen.</span><span class="sxs-lookup"><span data-stu-id="0db0b-113">Name.</span></span>|
|<span data-ttu-id="0db0b-114">Server</span><span class="sxs-lookup"><span data-stu-id="0db0b-114">servers</span></span>|<span data-ttu-id="0db0b-115">String collection</span><span class="sxs-lookup"><span data-stu-id="0db0b-115">String collection</span></span>|<span data-ttu-id="0db0b-116">Server.</span><span class="sxs-lookup"><span data-stu-id="0db0b-116">Servers.</span></span>|
|<span data-ttu-id="0db0b-117">proxyServerUri</span><span class="sxs-lookup"><span data-stu-id="0db0b-117">proxyServerUri</span></span>|<span data-ttu-id="0db0b-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0db0b-118">String</span></span>|<span data-ttu-id="0db0b-119">Proxy Server-URI.</span><span class="sxs-lookup"><span data-stu-id="0db0b-119">Proxy Server Uri.</span></span>|
|<span data-ttu-id="0db0b-120">autoTrigger</span><span class="sxs-lookup"><span data-stu-id="0db0b-120">autoTrigger</span></span>|<span data-ttu-id="0db0b-121">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0db0b-121">Boolean</span></span>|<span data-ttu-id="0db0b-122">Herstellen einer Verbindung mit dem VPN, wenn das Gerät eine Verbindung mit dieser Domäne herstellt: Standard false.</span><span class="sxs-lookup"><span data-stu-id="0db0b-122">Automatically connect to the VPN when the device connects to this domain: Default False.</span></span>|
|<span data-ttu-id="0db0b-123">persistent</span><span class="sxs-lookup"><span data-stu-id="0db0b-123">persistent</span></span>|<span data-ttu-id="0db0b-124">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0db0b-124">Boolean</span></span>|<span data-ttu-id="0db0b-125">Diese Regel auch dann aktiv halten, wenn das VPN nicht verbunden ist: Standard false</span><span class="sxs-lookup"><span data-stu-id="0db0b-125">Keep this rule active even when the VPN is not connected: Default False</span></span>|

## <a name="relationships"></a><span data-ttu-id="0db0b-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0db0b-126">Relationships</span></span>
<span data-ttu-id="0db0b-127">Keine</span><span class="sxs-lookup"><span data-stu-id="0db0b-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0db0b-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0db0b-128">JSON Representation</span></span>
<span data-ttu-id="0db0b-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0db0b-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnDnsRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnDnsRule",
  "name": "String",
  "servers": [
    "String"
  ],
  "proxyServerUri": "String",
  "autoTrigger": true,
  "persistent": true
}
```




