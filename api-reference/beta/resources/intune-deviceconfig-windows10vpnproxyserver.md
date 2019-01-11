---
title: Ressourcentyp windows10VpnProxyServer
description: VPN-Proxy-Server.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 231740bbeaa6757456fa684eb71a5b59ebd4adc6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872177"
---
# <a name="windows10vpnproxyserver-resource-type"></a><span data-ttu-id="c0c0d-103">Ressourcentyp windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="c0c0d-103">windows10VpnProxyServer resource type</span></span>

> <span data-ttu-id="c0c0d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c0c0d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0c0d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c0c0d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0c0d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c0c0d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0c0d-107">VPN-Proxy-Server.</span><span class="sxs-lookup"><span data-stu-id="c0c0d-107">VPN Proxy Server.</span></span>

<span data-ttu-id="c0c0d-108">Erbt vom [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="c0c0d-108">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c0c0d-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c0c0d-109">Properties</span></span>
|<span data-ttu-id="c0c0d-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c0c0d-110">Property</span></span>|<span data-ttu-id="c0c0d-111">Typ</span><span class="sxs-lookup"><span data-stu-id="c0c0d-111">Type</span></span>|<span data-ttu-id="c0c0d-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c0c0d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0c0d-113">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="c0c0d-113">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="c0c0d-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c0c0d-114">String</span></span>|<span data-ttu-id="c0c0d-115">Automatische Konfiguration Skript-Url des Proxys.</span><span class="sxs-lookup"><span data-stu-id="c0c0d-115">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="c0c0d-116">Geerbt von [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="c0c0d-116">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="c0c0d-117">address</span><span class="sxs-lookup"><span data-stu-id="c0c0d-117">address</span></span>|<span data-ttu-id="c0c0d-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c0c0d-118">String</span></span>|<span data-ttu-id="c0c0d-119">Adresse.</span><span class="sxs-lookup"><span data-stu-id="c0c0d-119">Address.</span></span> <span data-ttu-id="c0c0d-120">Geerbt von [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="c0c0d-120">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="c0c0d-121">port</span><span class="sxs-lookup"><span data-stu-id="c0c0d-121">port</span></span>|<span data-ttu-id="c0c0d-122">Int32</span><span class="sxs-lookup"><span data-stu-id="c0c0d-122">Int32</span></span>|<span data-ttu-id="c0c0d-123">Port.</span><span class="sxs-lookup"><span data-stu-id="c0c0d-123">Port.</span></span> <span data-ttu-id="c0c0d-124">Gültige Werte zwischen 0 und 65535 Inherited aus [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="c0c0d-124">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="c0c0d-125">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="c0c0d-125">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="c0c0d-126">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c0c0d-126">Boolean</span></span>|<span data-ttu-id="c0c0d-127">Proxyserver für lokale Adressen umgehen.</span><span class="sxs-lookup"><span data-stu-id="c0c0d-127">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0c0d-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c0c0d-128">Relationships</span></span>
<span data-ttu-id="c0c0d-129">Keine</span><span class="sxs-lookup"><span data-stu-id="c0c0d-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c0c0d-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c0c0d-130">JSON Representation</span></span>
<span data-ttu-id="c0c0d-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c0c0d-131">Here is a JSON representation of the resource.</span></span>
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





