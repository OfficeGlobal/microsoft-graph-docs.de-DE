---
title: Ressourcentyp vpnDnsRule
description: VPN-DNS-Regeldefinition.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ae6141cc0579840a23a28be2dce951c160f90248
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425582"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="f878e-103">Ressourcentyp vpnDnsRule</span><span class="sxs-lookup"><span data-stu-id="f878e-103">vpnDnsRule resource type</span></span>

> <span data-ttu-id="f878e-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="f878e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f878e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f878e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f878e-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f878e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f878e-107">VPN-DNS-Regeldefinition.</span><span class="sxs-lookup"><span data-stu-id="f878e-107">VPN DNS Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="f878e-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f878e-108">Properties</span></span>
|<span data-ttu-id="f878e-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f878e-109">Property</span></span>|<span data-ttu-id="f878e-110">Typ</span><span class="sxs-lookup"><span data-stu-id="f878e-110">Type</span></span>|<span data-ttu-id="f878e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f878e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f878e-112">name</span><span class="sxs-lookup"><span data-stu-id="f878e-112">name</span></span>|<span data-ttu-id="f878e-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f878e-113">String</span></span>|<span data-ttu-id="f878e-114">Name.</span><span class="sxs-lookup"><span data-stu-id="f878e-114">Name.</span></span>|
|<span data-ttu-id="f878e-115">Server</span><span class="sxs-lookup"><span data-stu-id="f878e-115">servers</span></span>|<span data-ttu-id="f878e-116">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="f878e-116">String collection</span></span>|<span data-ttu-id="f878e-117">Server.</span><span class="sxs-lookup"><span data-stu-id="f878e-117">Servers.</span></span>|
|<span data-ttu-id="f878e-118">proxyServerUri</span><span class="sxs-lookup"><span data-stu-id="f878e-118">proxyServerUri</span></span>|<span data-ttu-id="f878e-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f878e-119">String</span></span>|<span data-ttu-id="f878e-120">Proxy-Server-Uri.</span><span class="sxs-lookup"><span data-stu-id="f878e-120">Proxy Server Uri.</span></span>|
|<span data-ttu-id="f878e-121">autoTrigger</span><span class="sxs-lookup"><span data-stu-id="f878e-121">autoTrigger</span></span>|<span data-ttu-id="f878e-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="f878e-122">Boolean</span></span>|<span data-ttu-id="f878e-123">Automatisch mit dem VPN verbinden, wenn das Gerät an diese Domäne eine Verbindung herstellt: Standardeinstellung "false".</span><span class="sxs-lookup"><span data-stu-id="f878e-123">Automatically connect to the VPN when the device connects to this domain: Default False.</span></span>|
|<span data-ttu-id="f878e-124">persistent</span><span class="sxs-lookup"><span data-stu-id="f878e-124">persistent</span></span>|<span data-ttu-id="f878e-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="f878e-125">Boolean</span></span>|<span data-ttu-id="f878e-126">Diese Regel aktiv lassen, auch wenn das VPN nicht verbunden ist: Standardeinstellung "false"</span><span class="sxs-lookup"><span data-stu-id="f878e-126">Keep this rule active even when the VPN is not connected: Default False</span></span>|

## <a name="relationships"></a><span data-ttu-id="f878e-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f878e-127">Relationships</span></span>
<span data-ttu-id="f878e-128">Keine</span><span class="sxs-lookup"><span data-stu-id="f878e-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f878e-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f878e-129">JSON Representation</span></span>
<span data-ttu-id="f878e-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f878e-130">Here is a JSON representation of the resource.</span></span>
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




