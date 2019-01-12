---
title: windowsInformationProtectionProxiedDomainCollection-Ressourcentyp
description: Windows Information Protection – Proxydomänensammlung
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e5b7b1ece067f0f5e3672652c62913f1e39ef652
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976618"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="d47dd-103">windowsInformationProtectionProxiedDomainCollection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d47dd-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="d47dd-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d47dd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d47dd-105">Windows Information Protection – Proxydomänensammlung</span><span class="sxs-lookup"><span data-stu-id="d47dd-105">Windows Information Protection Proxied Domain Collection</span></span>
## <a name="properties"></a><span data-ttu-id="d47dd-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d47dd-106">Properties</span></span>
|<span data-ttu-id="d47dd-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d47dd-107">Property</span></span>|<span data-ttu-id="d47dd-108">Typ</span><span class="sxs-lookup"><span data-stu-id="d47dd-108">Type</span></span>|<span data-ttu-id="d47dd-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d47dd-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d47dd-110">displayName</span><span class="sxs-lookup"><span data-stu-id="d47dd-110">displayName</span></span>|<span data-ttu-id="d47dd-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d47dd-111">String</span></span>|<span data-ttu-id="d47dd-112">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="d47dd-112">Display name</span></span>|
|<span data-ttu-id="d47dd-113">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="d47dd-113">proxiedDomains</span></span>|<span data-ttu-id="d47dd-114">[proxiedDomain](../resources/intune-mam-proxieddomain.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d47dd-114">[proxiedDomain](../resources/intune-mam-proxieddomain.md) collection</span></span>|<span data-ttu-id="d47dd-115">Sammlung von Proxydomänen</span><span class="sxs-lookup"><span data-stu-id="d47dd-115">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="d47dd-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d47dd-116">Relationships</span></span>
<span data-ttu-id="d47dd-117">Keine</span><span class="sxs-lookup"><span data-stu-id="d47dd-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d47dd-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d47dd-118">JSON Representation</span></span>
<span data-ttu-id="d47dd-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d47dd-119">Here is a JSON representation of the resource.</span></span>
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



