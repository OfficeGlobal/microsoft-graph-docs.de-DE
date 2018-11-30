---
title: Ressourcentyp vpnProxyServer
description: VPN-Proxy-Server.
ms.openlocfilehash: 31e711475bf0f797eead80ca3fe2f3c9af8ba27f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059504"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="ec7f2-103">Ressourcentyp vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="ec7f2-103">vpnProxyServer resource type</span></span>

> <span data-ttu-id="ec7f2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ec7f2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ec7f2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ec7f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ec7f2-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ec7f2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ec7f2-107">VPN-Proxy-Server.</span><span class="sxs-lookup"><span data-stu-id="ec7f2-107">VPN Proxy Server.</span></span>
## <a name="properties"></a><span data-ttu-id="ec7f2-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ec7f2-108">Properties</span></span>
|<span data-ttu-id="ec7f2-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ec7f2-109">Property</span></span>|<span data-ttu-id="ec7f2-110">Typ</span><span class="sxs-lookup"><span data-stu-id="ec7f2-110">Type</span></span>|<span data-ttu-id="ec7f2-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ec7f2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec7f2-112">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="ec7f2-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="ec7f2-113">String</span><span class="sxs-lookup"><span data-stu-id="ec7f2-113">String</span></span>|<span data-ttu-id="ec7f2-114">Automatische Konfiguration Skript-Url des Proxys.</span><span class="sxs-lookup"><span data-stu-id="ec7f2-114">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="ec7f2-115">address</span><span class="sxs-lookup"><span data-stu-id="ec7f2-115">address</span></span>|<span data-ttu-id="ec7f2-116">String</span><span class="sxs-lookup"><span data-stu-id="ec7f2-116">String</span></span>|<span data-ttu-id="ec7f2-117">Adresse.</span><span class="sxs-lookup"><span data-stu-id="ec7f2-117">Address.</span></span>|
|<span data-ttu-id="ec7f2-118">port</span><span class="sxs-lookup"><span data-stu-id="ec7f2-118">port</span></span>|<span data-ttu-id="ec7f2-119">Int32</span><span class="sxs-lookup"><span data-stu-id="ec7f2-119">Int32</span></span>|<span data-ttu-id="ec7f2-120">Port.</span><span class="sxs-lookup"><span data-stu-id="ec7f2-120">Port.</span></span> <span data-ttu-id="ec7f2-121">Gültige Werte zwischen 0 und 65535</span><span class="sxs-lookup"><span data-stu-id="ec7f2-121">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec7f2-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ec7f2-122">Relationships</span></span>
<span data-ttu-id="ec7f2-123">Keine</span><span class="sxs-lookup"><span data-stu-id="ec7f2-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ec7f2-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ec7f2-124">JSON Representation</span></span>
<span data-ttu-id="ec7f2-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ec7f2-125">Here is a JSON representation of the resource.</span></span>
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





