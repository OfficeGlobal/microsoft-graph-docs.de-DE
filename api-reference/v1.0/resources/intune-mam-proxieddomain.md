---
title: proxiedDomain-Ressourcentyp
description: Proxydomäne
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: eff345414531b0ddda1600bb567aacd4a5436602
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871113"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="9e2fe-103">proxiedDomain-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9e2fe-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="9e2fe-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9e2fe-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e2fe-105">Proxydomäne</span><span class="sxs-lookup"><span data-stu-id="9e2fe-105">Proxied Domain</span></span>
## <a name="properties"></a><span data-ttu-id="9e2fe-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9e2fe-106">Properties</span></span>
|<span data-ttu-id="9e2fe-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9e2fe-107">Property</span></span>|<span data-ttu-id="9e2fe-108">Typ</span><span class="sxs-lookup"><span data-stu-id="9e2fe-108">Type</span></span>|<span data-ttu-id="9e2fe-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9e2fe-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e2fe-110">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="9e2fe-110">ipAddressOrFQDN</span></span>|<span data-ttu-id="9e2fe-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9e2fe-111">String</span></span>|<span data-ttu-id="9e2fe-112">Die IP-Adresse oder der FQDN</span><span class="sxs-lookup"><span data-stu-id="9e2fe-112">The IP address or FQDN</span></span>|
|<span data-ttu-id="9e2fe-113">Proxy</span><span class="sxs-lookup"><span data-stu-id="9e2fe-113">proxy</span></span>|<span data-ttu-id="9e2fe-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9e2fe-114">String</span></span>|<span data-ttu-id="9e2fe-115">Proxy-IP</span><span class="sxs-lookup"><span data-stu-id="9e2fe-115">Proxy IP</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e2fe-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9e2fe-116">Relationships</span></span>
<span data-ttu-id="9e2fe-117">Keine</span><span class="sxs-lookup"><span data-stu-id="9e2fe-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9e2fe-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9e2fe-118">JSON Representation</span></span>
<span data-ttu-id="9e2fe-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9e2fe-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.proxiedDomain"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.proxiedDomain",
  "ipAddressOrFQDN": "String",
  "proxy": "String"
}
```



