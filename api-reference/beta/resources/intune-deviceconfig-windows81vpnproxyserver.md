---
title: Ressourcentyp windows81VpnProxyServer
description: VPN-Proxy-Server.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d276ee7ac84bfe86c197025c05bf1a119b85e06c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917962"
---
# <a name="windows81vpnproxyserver-resource-type"></a><span data-ttu-id="96771-103">Ressourcentyp windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="96771-103">windows81VpnProxyServer resource type</span></span>

> <span data-ttu-id="96771-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="96771-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96771-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="96771-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="96771-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="96771-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96771-107">VPN-Proxy-Server.</span><span class="sxs-lookup"><span data-stu-id="96771-107">VPN Proxy Server.</span></span>

<span data-ttu-id="96771-108">Erbt vom [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="96771-108">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="96771-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="96771-109">Properties</span></span>
|<span data-ttu-id="96771-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="96771-110">Property</span></span>|<span data-ttu-id="96771-111">Typ</span><span class="sxs-lookup"><span data-stu-id="96771-111">Type</span></span>|<span data-ttu-id="96771-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96771-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96771-113">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="96771-113">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="96771-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="96771-114">String</span></span>|<span data-ttu-id="96771-115">Automatische Konfiguration Skript-Url des Proxys.</span><span class="sxs-lookup"><span data-stu-id="96771-115">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="96771-116">Geerbt von [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="96771-116">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="96771-117">address</span><span class="sxs-lookup"><span data-stu-id="96771-117">address</span></span>|<span data-ttu-id="96771-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="96771-118">String</span></span>|<span data-ttu-id="96771-119">Adresse.</span><span class="sxs-lookup"><span data-stu-id="96771-119">Address.</span></span> <span data-ttu-id="96771-120">Geerbt von [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="96771-120">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="96771-121">port</span><span class="sxs-lookup"><span data-stu-id="96771-121">port</span></span>|<span data-ttu-id="96771-122">Int32</span><span class="sxs-lookup"><span data-stu-id="96771-122">Int32</span></span>|<span data-ttu-id="96771-123">Port.</span><span class="sxs-lookup"><span data-stu-id="96771-123">Port.</span></span> <span data-ttu-id="96771-124">Gültige Werte zwischen 0 und 65535 Inherited aus [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="96771-124">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="96771-125">automaticallyDetectProxySettings</span><span class="sxs-lookup"><span data-stu-id="96771-125">automaticallyDetectProxySettings</span></span>|<span data-ttu-id="96771-126">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="96771-126">Boolean</span></span>|<span data-ttu-id="96771-127">Erkennen Sie Proxyeinstellungen automatisch.</span><span class="sxs-lookup"><span data-stu-id="96771-127">Automatically detect proxy settings.</span></span>|
|<span data-ttu-id="96771-128">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="96771-128">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="96771-129">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="96771-129">Boolean</span></span>|<span data-ttu-id="96771-130">Proxyserver für lokale Adressen umgehen.</span><span class="sxs-lookup"><span data-stu-id="96771-130">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96771-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="96771-131">Relationships</span></span>
<span data-ttu-id="96771-132">Keine</span><span class="sxs-lookup"><span data-stu-id="96771-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="96771-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="96771-133">JSON Representation</span></span>
<span data-ttu-id="96771-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="96771-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows81VpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows81VpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024,
  "automaticallyDetectProxySettings": true,
  "bypassProxyServerForLocalAddress": true
}
```





