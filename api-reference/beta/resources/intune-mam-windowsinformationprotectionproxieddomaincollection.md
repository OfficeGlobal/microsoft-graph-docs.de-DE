---
title: windowsInformationProtectionProxiedDomainCollection-Ressourcentyp
description: Windows Information Protection – Proxydomänensammlung
author: tfitzmac
ms.openlocfilehash: 3a385710dc38b5fb5927ee55e558fef67341585f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339347"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="15120-103">windowsInformationProtectionProxiedDomainCollection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="15120-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="15120-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="15120-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15120-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="15120-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15120-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="15120-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15120-107">Windows Information Protection – Proxydomänensammlung</span><span class="sxs-lookup"><span data-stu-id="15120-107">Windows Information Protection Proxied Domain Collection</span></span>
## <a name="properties"></a><span data-ttu-id="15120-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="15120-108">Properties</span></span>
|<span data-ttu-id="15120-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="15120-109">Property</span></span>|<span data-ttu-id="15120-110">Typ</span><span class="sxs-lookup"><span data-stu-id="15120-110">Type</span></span>|<span data-ttu-id="15120-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="15120-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15120-112">displayName</span><span class="sxs-lookup"><span data-stu-id="15120-112">displayName</span></span>|<span data-ttu-id="15120-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15120-113">String</span></span>|<span data-ttu-id="15120-114">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="15120-114">Display name</span></span>|
|<span data-ttu-id="15120-115">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="15120-115">proxiedDomains</span></span>|<span data-ttu-id="15120-116">[proxiedDomain](../resources/intune-shared-proxieddomain.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="15120-116">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="15120-117">Sammlung von Proxydomänen</span><span class="sxs-lookup"><span data-stu-id="15120-117">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="15120-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="15120-118">Relationships</span></span>
<span data-ttu-id="15120-119">Keine</span><span class="sxs-lookup"><span data-stu-id="15120-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="15120-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="15120-120">JSON Representation</span></span>
<span data-ttu-id="15120-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="15120-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
  "displayName": "String",
  "proxiedDomains": [
    {
      "@odata.type": "microsoft.graph.proxiedDomain",
      "ipAddressOrFQDN": "String",
      "proxy": "String"
    }
  ]
}
```





