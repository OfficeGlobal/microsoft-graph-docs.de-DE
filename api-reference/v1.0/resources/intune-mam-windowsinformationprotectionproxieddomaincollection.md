---
title: windowsInformationProtectionProxiedDomainCollection-Ressourcentyp
description: Windows Information Protection – Proxydomänensammlung
ms.openlocfilehash: b19709bff695d9184cda5adbffd9e0591e46db2b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019323"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="7d343-103">windowsInformationProtectionProxiedDomainCollection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7d343-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="7d343-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7d343-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d343-105">Windows Information Protection – Proxydomänensammlung</span><span class="sxs-lookup"><span data-stu-id="7d343-105">Windows Information Protection Proxied Domain Collection</span></span>
## <a name="properties"></a><span data-ttu-id="7d343-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7d343-106">Properties</span></span>
|<span data-ttu-id="7d343-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7d343-107">Property</span></span>|<span data-ttu-id="7d343-108">Typ</span><span class="sxs-lookup"><span data-stu-id="7d343-108">Type</span></span>|<span data-ttu-id="7d343-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7d343-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d343-110">displayName</span><span class="sxs-lookup"><span data-stu-id="7d343-110">displayName</span></span>|<span data-ttu-id="7d343-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7d343-111">String</span></span>|<span data-ttu-id="7d343-112">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="7d343-112">Display name</span></span>|
|<span data-ttu-id="7d343-113">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="7d343-113">proxiedDomains</span></span>|<span data-ttu-id="7d343-114">[proxiedDomain](../resources/intune-mam-proxieddomain.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="7d343-114">[proxiedDomain](../resources/intune-mam-proxieddomain.md) collection</span></span>|<span data-ttu-id="7d343-115">Sammlung von Proxydomänen</span><span class="sxs-lookup"><span data-stu-id="7d343-115">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d343-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7d343-116">Relationships</span></span>
<span data-ttu-id="7d343-117">Keine</span><span class="sxs-lookup"><span data-stu-id="7d343-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7d343-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7d343-118">JSON Representation</span></span>
<span data-ttu-id="7d343-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7d343-119">Here is a JSON representation of the resource.</span></span>
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



