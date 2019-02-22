---
title: vpnProxyServer-Ressourcentyp
description: VPN-Proxy Server.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b8a452cdde7c4c360107a67396d8f5ce49d6eb1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145276"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="92632-103">vpnProxyServer-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="92632-103">vpnProxyServer resource type</span></span>

> <span data-ttu-id="92632-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="92632-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92632-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="92632-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92632-106">VPN-Proxy Server.</span><span class="sxs-lookup"><span data-stu-id="92632-106">VPN Proxy Server.</span></span>

## <a name="properties"></a><span data-ttu-id="92632-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="92632-107">Properties</span></span>
|<span data-ttu-id="92632-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="92632-108">Property</span></span>|<span data-ttu-id="92632-109">Typ</span><span class="sxs-lookup"><span data-stu-id="92632-109">Type</span></span>|<span data-ttu-id="92632-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="92632-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92632-111">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="92632-111">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="92632-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="92632-112">String</span></span>|<span data-ttu-id="92632-113">URL des automatischen Konfigurationsskripts des Proxys.</span><span class="sxs-lookup"><span data-stu-id="92632-113">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="92632-114">address</span><span class="sxs-lookup"><span data-stu-id="92632-114">address</span></span>|<span data-ttu-id="92632-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="92632-115">String</span></span>|<span data-ttu-id="92632-116">Adresse.</span><span class="sxs-lookup"><span data-stu-id="92632-116">Address.</span></span>|
|<span data-ttu-id="92632-117">port</span><span class="sxs-lookup"><span data-stu-id="92632-117">port</span></span>|<span data-ttu-id="92632-118">Int32</span><span class="sxs-lookup"><span data-stu-id="92632-118">Int32</span></span>|<span data-ttu-id="92632-119">Port.</span><span class="sxs-lookup"><span data-stu-id="92632-119">Port.</span></span> <span data-ttu-id="92632-120">Gültige Werte 0 bis 65535</span><span class="sxs-lookup"><span data-stu-id="92632-120">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="92632-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="92632-121">Relationships</span></span>
<span data-ttu-id="92632-122">Keine</span><span class="sxs-lookup"><span data-stu-id="92632-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="92632-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="92632-123">JSON Representation</span></span>
<span data-ttu-id="92632-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="92632-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024
}
```




