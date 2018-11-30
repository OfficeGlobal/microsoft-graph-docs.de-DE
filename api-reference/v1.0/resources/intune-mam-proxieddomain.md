---
title: proxiedDomain-Ressourcentyp
description: Proxydomäne
ms.openlocfilehash: d73ed20341a7de025f6f2d39536a1e791b978f55
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018557"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="89141-103">proxiedDomain-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="89141-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="89141-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="89141-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89141-105">Proxydomäne</span><span class="sxs-lookup"><span data-stu-id="89141-105">Proxied Domain</span></span>
## <a name="properties"></a><span data-ttu-id="89141-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="89141-106">Properties</span></span>
|<span data-ttu-id="89141-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="89141-107">Property</span></span>|<span data-ttu-id="89141-108">Typ</span><span class="sxs-lookup"><span data-stu-id="89141-108">Type</span></span>|<span data-ttu-id="89141-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="89141-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89141-110">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="89141-110">ipAddressOrFQDN</span></span>|<span data-ttu-id="89141-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="89141-111">String</span></span>|<span data-ttu-id="89141-112">Die IP-Adresse oder der FQDN</span><span class="sxs-lookup"><span data-stu-id="89141-112">The IP address or FQDN</span></span>|
|<span data-ttu-id="89141-113">Proxy</span><span class="sxs-lookup"><span data-stu-id="89141-113">proxy</span></span>|<span data-ttu-id="89141-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="89141-114">String</span></span>|<span data-ttu-id="89141-115">Proxy-IP</span><span class="sxs-lookup"><span data-stu-id="89141-115">Proxy IP</span></span>|

## <a name="relationships"></a><span data-ttu-id="89141-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="89141-116">Relationships</span></span>
<span data-ttu-id="89141-117">Keine</span><span class="sxs-lookup"><span data-stu-id="89141-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="89141-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="89141-118">JSON Representation</span></span>
<span data-ttu-id="89141-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="89141-119">Here is a JSON representation of the resource.</span></span>
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



