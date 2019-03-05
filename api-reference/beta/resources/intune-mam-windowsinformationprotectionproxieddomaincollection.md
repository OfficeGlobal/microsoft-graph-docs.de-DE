---
title: windowsInformationProtectionProxiedDomainCollection-Ressourcentyp
description: Windows Information Protection – Proxydomänensammlung
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c03eba4089fc984478854cd50b378c0f2d9b155
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143407"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="16719-103">windowsInformationProtectionProxiedDomainCollection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="16719-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="16719-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="16719-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16719-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="16719-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16719-106">Windows Information Protection – Proxydomänensammlung</span><span class="sxs-lookup"><span data-stu-id="16719-106">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="16719-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="16719-107">Properties</span></span>
|<span data-ttu-id="16719-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="16719-108">Property</span></span>|<span data-ttu-id="16719-109">Typ</span><span class="sxs-lookup"><span data-stu-id="16719-109">Type</span></span>|<span data-ttu-id="16719-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16719-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16719-111">displayName</span><span class="sxs-lookup"><span data-stu-id="16719-111">displayName</span></span>|<span data-ttu-id="16719-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="16719-112">String</span></span>|<span data-ttu-id="16719-113">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="16719-113">Display name</span></span>|
|<span data-ttu-id="16719-114">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="16719-114">proxiedDomains</span></span>|<span data-ttu-id="16719-115">[proxiedDomain](../resources/intune-shared-proxieddomain.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="16719-115">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="16719-116">Sammlung von Proxydomänen</span><span class="sxs-lookup"><span data-stu-id="16719-116">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="16719-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="16719-117">Relationships</span></span>
<span data-ttu-id="16719-118">Keine</span><span class="sxs-lookup"><span data-stu-id="16719-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="16719-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="16719-119">JSON Representation</span></span>
<span data-ttu-id="16719-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="16719-120">Here is a JSON representation of the resource.</span></span>
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




