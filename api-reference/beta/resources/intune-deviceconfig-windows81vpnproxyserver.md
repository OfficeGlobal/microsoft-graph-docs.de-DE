---
title: Ressourcentyp windows81VpnProxyServer
description: VPN-Proxy-Server.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a400ed128a80e6fae11f090f7cdd445fe8c174b0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398891"
---
# <a name="windows81vpnproxyserver-resource-type"></a><span data-ttu-id="79363-103">Ressourcentyp windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="79363-103">windows81VpnProxyServer resource type</span></span>

> <span data-ttu-id="79363-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="79363-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="79363-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="79363-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="79363-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="79363-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79363-107">VPN-Proxy-Server.</span><span class="sxs-lookup"><span data-stu-id="79363-107">VPN Proxy Server.</span></span>


<span data-ttu-id="79363-108">Erbt vom [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="79363-108">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="79363-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="79363-109">Properties</span></span>
|<span data-ttu-id="79363-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="79363-110">Property</span></span>|<span data-ttu-id="79363-111">Typ</span><span class="sxs-lookup"><span data-stu-id="79363-111">Type</span></span>|<span data-ttu-id="79363-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="79363-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79363-113">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="79363-113">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="79363-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="79363-114">String</span></span>|<span data-ttu-id="79363-115">Automatische Konfiguration Skript-Url des Proxys.</span><span class="sxs-lookup"><span data-stu-id="79363-115">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="79363-116">Geerbt von [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="79363-116">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="79363-117">address</span><span class="sxs-lookup"><span data-stu-id="79363-117">address</span></span>|<span data-ttu-id="79363-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="79363-118">String</span></span>|<span data-ttu-id="79363-119">Adresse.</span><span class="sxs-lookup"><span data-stu-id="79363-119">Address.</span></span> <span data-ttu-id="79363-120">Geerbt von [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="79363-120">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="79363-121">port</span><span class="sxs-lookup"><span data-stu-id="79363-121">port</span></span>|<span data-ttu-id="79363-122">Int32</span><span class="sxs-lookup"><span data-stu-id="79363-122">Int32</span></span>|<span data-ttu-id="79363-123">Port.</span><span class="sxs-lookup"><span data-stu-id="79363-123">Port.</span></span> <span data-ttu-id="79363-124">Gültige Werte zwischen 0 und 65535 Inherited aus [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="79363-124">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="79363-125">automaticallyDetectProxySettings</span><span class="sxs-lookup"><span data-stu-id="79363-125">automaticallyDetectProxySettings</span></span>|<span data-ttu-id="79363-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="79363-126">Boolean</span></span>|<span data-ttu-id="79363-127">Erkennen Sie Proxyeinstellungen automatisch.</span><span class="sxs-lookup"><span data-stu-id="79363-127">Automatically detect proxy settings.</span></span>|
|<span data-ttu-id="79363-128">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="79363-128">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="79363-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="79363-129">Boolean</span></span>|<span data-ttu-id="79363-130">Proxyserver für lokale Adressen umgehen.</span><span class="sxs-lookup"><span data-stu-id="79363-130">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="79363-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="79363-131">Relationships</span></span>
<span data-ttu-id="79363-132">Keine</span><span class="sxs-lookup"><span data-stu-id="79363-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="79363-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="79363-133">JSON Representation</span></span>
<span data-ttu-id="79363-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="79363-134">Here is a JSON representation of the resource.</span></span>
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




