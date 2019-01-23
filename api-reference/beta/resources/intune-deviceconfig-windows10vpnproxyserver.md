---
title: Ressourcentyp windows10VpnProxyServer
description: VPN-Proxy-Server.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d4f8975a08e60105c37e0959ac72e24a1dd639cd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407123"
---
# <a name="windows10vpnproxyserver-resource-type"></a><span data-ttu-id="f39e0-103">Ressourcentyp windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="f39e0-103">windows10VpnProxyServer resource type</span></span>

> <span data-ttu-id="f39e0-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="f39e0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f39e0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f39e0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f39e0-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f39e0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f39e0-107">VPN-Proxy-Server.</span><span class="sxs-lookup"><span data-stu-id="f39e0-107">VPN Proxy Server.</span></span>


<span data-ttu-id="f39e0-108">Erbt vom [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="f39e0-108">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f39e0-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f39e0-109">Properties</span></span>
|<span data-ttu-id="f39e0-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f39e0-110">Property</span></span>|<span data-ttu-id="f39e0-111">Typ</span><span class="sxs-lookup"><span data-stu-id="f39e0-111">Type</span></span>|<span data-ttu-id="f39e0-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f39e0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f39e0-113">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="f39e0-113">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="f39e0-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f39e0-114">String</span></span>|<span data-ttu-id="f39e0-115">Automatische Konfiguration Skript-Url des Proxys.</span><span class="sxs-lookup"><span data-stu-id="f39e0-115">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="f39e0-116">Geerbt von [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="f39e0-116">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="f39e0-117">address</span><span class="sxs-lookup"><span data-stu-id="f39e0-117">address</span></span>|<span data-ttu-id="f39e0-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f39e0-118">String</span></span>|<span data-ttu-id="f39e0-119">Adresse.</span><span class="sxs-lookup"><span data-stu-id="f39e0-119">Address.</span></span> <span data-ttu-id="f39e0-120">Geerbt von [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="f39e0-120">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="f39e0-121">port</span><span class="sxs-lookup"><span data-stu-id="f39e0-121">port</span></span>|<span data-ttu-id="f39e0-122">Int32</span><span class="sxs-lookup"><span data-stu-id="f39e0-122">Int32</span></span>|<span data-ttu-id="f39e0-123">Port.</span><span class="sxs-lookup"><span data-stu-id="f39e0-123">Port.</span></span> <span data-ttu-id="f39e0-124">Gültige Werte zwischen 0 und 65535 Inherited aus [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="f39e0-124">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="f39e0-125">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="f39e0-125">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="f39e0-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="f39e0-126">Boolean</span></span>|<span data-ttu-id="f39e0-127">Proxyserver für lokale Adressen umgehen.</span><span class="sxs-lookup"><span data-stu-id="f39e0-127">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f39e0-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f39e0-128">Relationships</span></span>
<span data-ttu-id="f39e0-129">Keine</span><span class="sxs-lookup"><span data-stu-id="f39e0-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f39e0-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f39e0-130">JSON Representation</span></span>
<span data-ttu-id="f39e0-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f39e0-131">Here is a JSON representation of the resource.</span></span>
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




