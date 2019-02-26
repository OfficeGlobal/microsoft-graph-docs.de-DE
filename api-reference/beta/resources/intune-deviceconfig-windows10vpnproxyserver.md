---
title: windows10VpnProxyServer-Ressourcentyp
description: VPN-Proxy Server.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4686049e2f3525409e81ec1492dcb052ab9f3657
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140691"
---
# <a name="windows10vpnproxyserver-resource-type"></a><span data-ttu-id="5363d-103">windows10VpnProxyServer-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5363d-103">windows10VpnProxyServer resource type</span></span>

> <span data-ttu-id="5363d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5363d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5363d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5363d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5363d-106">VPN-Proxy Server.</span><span class="sxs-lookup"><span data-stu-id="5363d-106">VPN Proxy Server.</span></span>


<span data-ttu-id="5363d-107">Erbt von [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="5363d-107">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5363d-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5363d-108">Properties</span></span>
|<span data-ttu-id="5363d-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5363d-109">Property</span></span>|<span data-ttu-id="5363d-110">Typ</span><span class="sxs-lookup"><span data-stu-id="5363d-110">Type</span></span>|<span data-ttu-id="5363d-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5363d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5363d-112">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="5363d-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="5363d-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5363d-113">String</span></span>|<span data-ttu-id="5363d-114">URL des automatischen Konfigurationsskripts des Proxys.</span><span class="sxs-lookup"><span data-stu-id="5363d-114">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="5363d-115">Geerbt von [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="5363d-115">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="5363d-116">address</span><span class="sxs-lookup"><span data-stu-id="5363d-116">address</span></span>|<span data-ttu-id="5363d-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5363d-117">String</span></span>|<span data-ttu-id="5363d-118">Adresse.</span><span class="sxs-lookup"><span data-stu-id="5363d-118">Address.</span></span> <span data-ttu-id="5363d-119">Geerbt von [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="5363d-119">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="5363d-120">port</span><span class="sxs-lookup"><span data-stu-id="5363d-120">port</span></span>|<span data-ttu-id="5363d-121">Int32</span><span class="sxs-lookup"><span data-stu-id="5363d-121">Int32</span></span>|<span data-ttu-id="5363d-122">Port.</span><span class="sxs-lookup"><span data-stu-id="5363d-122">Port.</span></span> <span data-ttu-id="5363d-123">Gültige Werte 0 bis 65535 geerbt von [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="5363d-123">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="5363d-124">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="5363d-124">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="5363d-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="5363d-125">Boolean</span></span>|<span data-ttu-id="5363d-126">Umgehen des Proxyservers für die lokale Adresse.</span><span class="sxs-lookup"><span data-stu-id="5363d-126">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5363d-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5363d-127">Relationships</span></span>
<span data-ttu-id="5363d-128">Keine</span><span class="sxs-lookup"><span data-stu-id="5363d-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5363d-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5363d-129">JSON Representation</span></span>
<span data-ttu-id="5363d-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5363d-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10VpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10VpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024,
  "bypassProxyServerForLocalAddress": true
}
```




