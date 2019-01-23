---
title: Ressourcentyp vpnProxyServer
description: VPN-Proxy-Server.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 676e56771f021a79179e268280f5e3190754eef2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425673"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="87381-103">Ressourcentyp vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="87381-103">vpnProxyServer resource type</span></span>

> <span data-ttu-id="87381-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="87381-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="87381-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="87381-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="87381-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="87381-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87381-107">VPN-Proxy-Server.</span><span class="sxs-lookup"><span data-stu-id="87381-107">VPN Proxy Server.</span></span>

## <a name="properties"></a><span data-ttu-id="87381-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="87381-108">Properties</span></span>
|<span data-ttu-id="87381-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="87381-109">Property</span></span>|<span data-ttu-id="87381-110">Typ</span><span class="sxs-lookup"><span data-stu-id="87381-110">Type</span></span>|<span data-ttu-id="87381-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87381-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87381-112">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="87381-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="87381-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="87381-113">String</span></span>|<span data-ttu-id="87381-114">Automatische Konfiguration Skript-Url des Proxys.</span><span class="sxs-lookup"><span data-stu-id="87381-114">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="87381-115">address</span><span class="sxs-lookup"><span data-stu-id="87381-115">address</span></span>|<span data-ttu-id="87381-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="87381-116">String</span></span>|<span data-ttu-id="87381-117">Adresse.</span><span class="sxs-lookup"><span data-stu-id="87381-117">Address.</span></span>|
|<span data-ttu-id="87381-118">port</span><span class="sxs-lookup"><span data-stu-id="87381-118">port</span></span>|<span data-ttu-id="87381-119">Int32</span><span class="sxs-lookup"><span data-stu-id="87381-119">Int32</span></span>|<span data-ttu-id="87381-120">Port.</span><span class="sxs-lookup"><span data-stu-id="87381-120">Port.</span></span> <span data-ttu-id="87381-121">Gültige Werte zwischen 0 und 65535</span><span class="sxs-lookup"><span data-stu-id="87381-121">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="87381-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="87381-122">Relationships</span></span>
<span data-ttu-id="87381-123">Keine</span><span class="sxs-lookup"><span data-stu-id="87381-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="87381-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="87381-124">JSON Representation</span></span>
<span data-ttu-id="87381-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="87381-125">Here is a JSON representation of the resource.</span></span>
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




