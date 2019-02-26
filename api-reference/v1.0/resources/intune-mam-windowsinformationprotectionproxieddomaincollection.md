---
title: windowsInformationProtectionProxiedDomainCollection-Ressourcentyp
description: Windows Information Protection – Proxydomänensammlung
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 026a69dc7697a0b779d72dfcab1695cf8c219d83
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264330"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="7221b-103">windowsInformationProtectionProxiedDomainCollection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7221b-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="7221b-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7221b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7221b-105">Windows Information Protection – Proxydomänensammlung</span><span class="sxs-lookup"><span data-stu-id="7221b-105">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="7221b-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7221b-106">Properties</span></span>
|<span data-ttu-id="7221b-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7221b-107">Property</span></span>|<span data-ttu-id="7221b-108">Typ</span><span class="sxs-lookup"><span data-stu-id="7221b-108">Type</span></span>|<span data-ttu-id="7221b-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7221b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7221b-110">displayName</span><span class="sxs-lookup"><span data-stu-id="7221b-110">displayName</span></span>|<span data-ttu-id="7221b-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7221b-111">String</span></span>|<span data-ttu-id="7221b-112">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="7221b-112">Display name</span></span>|
|<span data-ttu-id="7221b-113">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="7221b-113">proxiedDomains</span></span>|<span data-ttu-id="7221b-114">[proxiedDomain](../resources/intune-mam-proxieddomain.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="7221b-114">[proxiedDomain](../resources/intune-mam-proxieddomain.md) collection</span></span>|<span data-ttu-id="7221b-115">Sammlung von Proxydomänen</span><span class="sxs-lookup"><span data-stu-id="7221b-115">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="7221b-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7221b-116">Relationships</span></span>
<span data-ttu-id="7221b-117">Keine</span><span class="sxs-lookup"><span data-stu-id="7221b-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7221b-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7221b-118">JSON Representation</span></span>
<span data-ttu-id="7221b-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7221b-119">Here is a JSON representation of the resource.</span></span>
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



