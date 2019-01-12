---
title: Ressourcentyp vpnDnsRule
description: VPN-DNS-Regeldefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3c928542f749973ac3abea041c8ca60ee74ff8fe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964739"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="00995-103">Ressourcentyp vpnDnsRule</span><span class="sxs-lookup"><span data-stu-id="00995-103">vpnDnsRule resource type</span></span>

> <span data-ttu-id="00995-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="00995-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00995-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="00995-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="00995-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="00995-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00995-107">VPN-DNS-Regeldefinition.</span><span class="sxs-lookup"><span data-stu-id="00995-107">VPN DNS Rule definition.</span></span>
## <a name="properties"></a><span data-ttu-id="00995-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="00995-108">Properties</span></span>
|<span data-ttu-id="00995-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="00995-109">Property</span></span>|<span data-ttu-id="00995-110">Typ</span><span class="sxs-lookup"><span data-stu-id="00995-110">Type</span></span>|<span data-ttu-id="00995-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="00995-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00995-112">name</span><span class="sxs-lookup"><span data-stu-id="00995-112">name</span></span>|<span data-ttu-id="00995-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="00995-113">String</span></span>|<span data-ttu-id="00995-114">Name.</span><span class="sxs-lookup"><span data-stu-id="00995-114">Name.</span></span>|
|<span data-ttu-id="00995-115">Server</span><span class="sxs-lookup"><span data-stu-id="00995-115">servers</span></span>|<span data-ttu-id="00995-116">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="00995-116">String collection</span></span>|<span data-ttu-id="00995-117">Server.</span><span class="sxs-lookup"><span data-stu-id="00995-117">Servers.</span></span>|
|<span data-ttu-id="00995-118">proxyServerUri</span><span class="sxs-lookup"><span data-stu-id="00995-118">proxyServerUri</span></span>|<span data-ttu-id="00995-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="00995-119">String</span></span>|<span data-ttu-id="00995-120">Proxy-Server-Uri.</span><span class="sxs-lookup"><span data-stu-id="00995-120">Proxy Server Uri.</span></span>|

## <a name="relationships"></a><span data-ttu-id="00995-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="00995-121">Relationships</span></span>
<span data-ttu-id="00995-122">Keine</span><span class="sxs-lookup"><span data-stu-id="00995-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="00995-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="00995-123">JSON Representation</span></span>
<span data-ttu-id="00995-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="00995-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnDnsRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnDnsRule",
  "name": "String",
  "servers": [
    "String"
  ],
  "proxyServerUri": "String"
}
```





