---
title: windows81VpnProxyServer-Ressourcentyp
description: VPN-Proxy Server.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a6783502079ab3ce3adf3f8133662ab3eab578bd
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145206"
---
# <a name="windows81vpnproxyserver-resource-type"></a><span data-ttu-id="a8b76-103">windows81VpnProxyServer-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a8b76-103">windows81VpnProxyServer resource type</span></span>

> <span data-ttu-id="a8b76-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a8b76-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8b76-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a8b76-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8b76-106">VPN-Proxy Server.</span><span class="sxs-lookup"><span data-stu-id="a8b76-106">VPN Proxy Server.</span></span>


<span data-ttu-id="a8b76-107">Erbt von [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="a8b76-107">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a8b76-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a8b76-108">Properties</span></span>
|<span data-ttu-id="a8b76-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a8b76-109">Property</span></span>|<span data-ttu-id="a8b76-110">Typ</span><span class="sxs-lookup"><span data-stu-id="a8b76-110">Type</span></span>|<span data-ttu-id="a8b76-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8b76-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8b76-112">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="a8b76-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="a8b76-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a8b76-113">String</span></span>|<span data-ttu-id="a8b76-114">URL des automatischen Konfigurationsskripts des Proxys.</span><span class="sxs-lookup"><span data-stu-id="a8b76-114">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="a8b76-115">Geerbt von [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="a8b76-115">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="a8b76-116">address</span><span class="sxs-lookup"><span data-stu-id="a8b76-116">address</span></span>|<span data-ttu-id="a8b76-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a8b76-117">String</span></span>|<span data-ttu-id="a8b76-118">Adresse.</span><span class="sxs-lookup"><span data-stu-id="a8b76-118">Address.</span></span> <span data-ttu-id="a8b76-119">Geerbt von [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="a8b76-119">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="a8b76-120">port</span><span class="sxs-lookup"><span data-stu-id="a8b76-120">port</span></span>|<span data-ttu-id="a8b76-121">Int32</span><span class="sxs-lookup"><span data-stu-id="a8b76-121">Int32</span></span>|<span data-ttu-id="a8b76-122">Port.</span><span class="sxs-lookup"><span data-stu-id="a8b76-122">Port.</span></span> <span data-ttu-id="a8b76-123">Gültige Werte 0 bis 65535 geerbt von [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="a8b76-123">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="a8b76-124">automaticallyDetectProxySettings</span><span class="sxs-lookup"><span data-stu-id="a8b76-124">automaticallyDetectProxySettings</span></span>|<span data-ttu-id="a8b76-125">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a8b76-125">Boolean</span></span>|<span data-ttu-id="a8b76-126">Proxyeinstellungen werden automatisch ermittelt.</span><span class="sxs-lookup"><span data-stu-id="a8b76-126">Automatically detect proxy settings.</span></span>|
|<span data-ttu-id="a8b76-127">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="a8b76-127">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="a8b76-128">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a8b76-128">Boolean</span></span>|<span data-ttu-id="a8b76-129">Umgehen des Proxyservers für die lokale Adresse.</span><span class="sxs-lookup"><span data-stu-id="a8b76-129">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8b76-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a8b76-130">Relationships</span></span>
<span data-ttu-id="a8b76-131">Keine</span><span class="sxs-lookup"><span data-stu-id="a8b76-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8b76-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a8b76-132">JSON Representation</span></span>
<span data-ttu-id="a8b76-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a8b76-133">Here is a JSON representation of the resource.</span></span>
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




