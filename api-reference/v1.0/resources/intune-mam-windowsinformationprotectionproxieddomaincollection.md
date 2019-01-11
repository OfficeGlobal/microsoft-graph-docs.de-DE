---
title: windowsInformationProtectionProxiedDomainCollection-Ressourcentyp
description: Windows Information Protection – Proxydomänensammlung
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: dfc07b47115e4e5ce4be959ac7867a2963021abf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822099"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="0b068-103">windowsInformationProtectionProxiedDomainCollection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0b068-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="0b068-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0b068-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0b068-105">Windows Information Protection – Proxydomänensammlung</span><span class="sxs-lookup"><span data-stu-id="0b068-105">Windows Information Protection Proxied Domain Collection</span></span>
## <a name="properties"></a><span data-ttu-id="0b068-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0b068-106">Properties</span></span>
|<span data-ttu-id="0b068-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0b068-107">Property</span></span>|<span data-ttu-id="0b068-108">Typ</span><span class="sxs-lookup"><span data-stu-id="0b068-108">Type</span></span>|<span data-ttu-id="0b068-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0b068-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b068-110">displayName</span><span class="sxs-lookup"><span data-stu-id="0b068-110">displayName</span></span>|<span data-ttu-id="0b068-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0b068-111">String</span></span>|<span data-ttu-id="0b068-112">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="0b068-112">Display name</span></span>|
|<span data-ttu-id="0b068-113">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="0b068-113">proxiedDomains</span></span>|<span data-ttu-id="0b068-114">[proxiedDomain](../resources/intune-mam-proxieddomain.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="0b068-114">[proxiedDomain](../resources/intune-mam-proxieddomain.md) collection</span></span>|<span data-ttu-id="0b068-115">Sammlung von Proxydomänen</span><span class="sxs-lookup"><span data-stu-id="0b068-115">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b068-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0b068-116">Relationships</span></span>
<span data-ttu-id="0b068-117">Keine</span><span class="sxs-lookup"><span data-stu-id="0b068-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0b068-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0b068-118">JSON Representation</span></span>
<span data-ttu-id="0b068-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0b068-119">Here is a JSON representation of the resource.</span></span>
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



