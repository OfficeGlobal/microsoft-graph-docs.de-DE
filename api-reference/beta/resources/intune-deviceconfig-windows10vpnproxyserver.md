---
title: Ressourcentyp windows10VpnProxyServer
description: VPN-Proxy-Server.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a4b34d105900478a1bcbc811e782e1ceaf94f251
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912274"
---
# <a name="windows10vpnproxyserver-resource-type"></a><span data-ttu-id="dbfa7-103">Ressourcentyp windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="dbfa7-103">windows10VpnProxyServer resource type</span></span>

> <span data-ttu-id="dbfa7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dbfa7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dbfa7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dbfa7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dbfa7-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="dbfa7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dbfa7-107">VPN-Proxy-Server.</span><span class="sxs-lookup"><span data-stu-id="dbfa7-107">VPN Proxy Server.</span></span>

<span data-ttu-id="dbfa7-108">Erbt vom [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="dbfa7-108">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dbfa7-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dbfa7-109">Properties</span></span>
|<span data-ttu-id="dbfa7-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dbfa7-110">Property</span></span>|<span data-ttu-id="dbfa7-111">Typ</span><span class="sxs-lookup"><span data-stu-id="dbfa7-111">Type</span></span>|<span data-ttu-id="dbfa7-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dbfa7-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbfa7-113">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="dbfa7-113">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="dbfa7-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dbfa7-114">String</span></span>|<span data-ttu-id="dbfa7-115">Automatische Konfiguration Skript-Url des Proxys.</span><span class="sxs-lookup"><span data-stu-id="dbfa7-115">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="dbfa7-116">Geerbt von [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="dbfa7-116">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="dbfa7-117">address</span><span class="sxs-lookup"><span data-stu-id="dbfa7-117">address</span></span>|<span data-ttu-id="dbfa7-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dbfa7-118">String</span></span>|<span data-ttu-id="dbfa7-119">Adresse.</span><span class="sxs-lookup"><span data-stu-id="dbfa7-119">Address.</span></span> <span data-ttu-id="dbfa7-120">Geerbt von [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="dbfa7-120">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="dbfa7-121">port</span><span class="sxs-lookup"><span data-stu-id="dbfa7-121">port</span></span>|<span data-ttu-id="dbfa7-122">Int32</span><span class="sxs-lookup"><span data-stu-id="dbfa7-122">Int32</span></span>|<span data-ttu-id="dbfa7-123">Port.</span><span class="sxs-lookup"><span data-stu-id="dbfa7-123">Port.</span></span> <span data-ttu-id="dbfa7-124">Gültige Werte zwischen 0 und 65535 Inherited aus [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="dbfa7-124">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="dbfa7-125">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="dbfa7-125">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="dbfa7-126">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="dbfa7-126">Boolean</span></span>|<span data-ttu-id="dbfa7-127">Proxyserver für lokale Adressen umgehen.</span><span class="sxs-lookup"><span data-stu-id="dbfa7-127">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dbfa7-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="dbfa7-128">Relationships</span></span>
<span data-ttu-id="dbfa7-129">Keine</span><span class="sxs-lookup"><span data-stu-id="dbfa7-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dbfa7-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="dbfa7-130">JSON Representation</span></span>
<span data-ttu-id="dbfa7-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="dbfa7-131">Here is a JSON representation of the resource.</span></span>
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





