---
title: windowsInformationProtectionProxiedDomainCollection-Ressourcentyp
description: Windows Information Protection – Proxydomänensammlung
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c65a4b6a94f317c5d75b440aeef7fe387496be32
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421676"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="3ed4c-103">windowsInformationProtectionProxiedDomainCollection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3ed4c-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="3ed4c-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="3ed4c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3ed4c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3ed4c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3ed4c-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3ed4c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ed4c-107">Windows Information Protection – Proxydomänensammlung</span><span class="sxs-lookup"><span data-stu-id="3ed4c-107">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="3ed4c-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3ed4c-108">Properties</span></span>
|<span data-ttu-id="3ed4c-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3ed4c-109">Property</span></span>|<span data-ttu-id="3ed4c-110">Typ</span><span class="sxs-lookup"><span data-stu-id="3ed4c-110">Type</span></span>|<span data-ttu-id="3ed4c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3ed4c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ed4c-112">displayName</span><span class="sxs-lookup"><span data-stu-id="3ed4c-112">displayName</span></span>|<span data-ttu-id="3ed4c-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3ed4c-113">String</span></span>|<span data-ttu-id="3ed4c-114">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="3ed4c-114">Display name</span></span>|
|<span data-ttu-id="3ed4c-115">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="3ed4c-115">proxiedDomains</span></span>|<span data-ttu-id="3ed4c-116">[proxiedDomain](../resources/intune-shared-proxieddomain.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="3ed4c-116">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="3ed4c-117">Sammlung von Proxydomänen</span><span class="sxs-lookup"><span data-stu-id="3ed4c-117">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ed4c-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3ed4c-118">Relationships</span></span>
<span data-ttu-id="3ed4c-119">Keine</span><span class="sxs-lookup"><span data-stu-id="3ed4c-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ed4c-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3ed4c-120">JSON Representation</span></span>
<span data-ttu-id="3ed4c-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3ed4c-121">Here is a JSON representation of the resource.</span></span>
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




