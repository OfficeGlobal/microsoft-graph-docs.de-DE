---
title: Ressourcentyp vpnProxyServer
description: VPN-Proxy-Server.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 727d26af7f2c1801cd06fc98949109efec267f27
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955352"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="6d2e7-103">Ressourcentyp vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="6d2e7-103">vpnProxyServer resource type</span></span>

> <span data-ttu-id="6d2e7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6d2e7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6d2e7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6d2e7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6d2e7-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6d2e7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6d2e7-107">VPN-Proxy-Server.</span><span class="sxs-lookup"><span data-stu-id="6d2e7-107">VPN Proxy Server.</span></span>
## <a name="properties"></a><span data-ttu-id="6d2e7-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6d2e7-108">Properties</span></span>
|<span data-ttu-id="6d2e7-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6d2e7-109">Property</span></span>|<span data-ttu-id="6d2e7-110">Typ</span><span class="sxs-lookup"><span data-stu-id="6d2e7-110">Type</span></span>|<span data-ttu-id="6d2e7-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6d2e7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d2e7-112">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="6d2e7-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="6d2e7-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6d2e7-113">String</span></span>|<span data-ttu-id="6d2e7-114">Automatische Konfiguration Skript-Url des Proxys.</span><span class="sxs-lookup"><span data-stu-id="6d2e7-114">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="6d2e7-115">address</span><span class="sxs-lookup"><span data-stu-id="6d2e7-115">address</span></span>|<span data-ttu-id="6d2e7-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6d2e7-116">String</span></span>|<span data-ttu-id="6d2e7-117">Adresse.</span><span class="sxs-lookup"><span data-stu-id="6d2e7-117">Address.</span></span>|
|<span data-ttu-id="6d2e7-118">port</span><span class="sxs-lookup"><span data-stu-id="6d2e7-118">port</span></span>|<span data-ttu-id="6d2e7-119">Int32</span><span class="sxs-lookup"><span data-stu-id="6d2e7-119">Int32</span></span>|<span data-ttu-id="6d2e7-120">Port.</span><span class="sxs-lookup"><span data-stu-id="6d2e7-120">Port.</span></span> <span data-ttu-id="6d2e7-121">Gültige Werte zwischen 0 und 65535</span><span class="sxs-lookup"><span data-stu-id="6d2e7-121">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d2e7-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6d2e7-122">Relationships</span></span>
<span data-ttu-id="6d2e7-123">Keine</span><span class="sxs-lookup"><span data-stu-id="6d2e7-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6d2e7-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6d2e7-124">JSON Representation</span></span>
<span data-ttu-id="6d2e7-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6d2e7-125">Here is a JSON representation of the resource.</span></span>
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





