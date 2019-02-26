---
title: proxiedDomain-Ressourcentyp
description: Proxydomäne
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b28271308f5256d034de3b4704353aa0471aeb29
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264043"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="5f903-103">proxiedDomain-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5f903-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="5f903-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5f903-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f903-105">Proxydomäne</span><span class="sxs-lookup"><span data-stu-id="5f903-105">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="5f903-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5f903-106">Properties</span></span>
|<span data-ttu-id="5f903-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5f903-107">Property</span></span>|<span data-ttu-id="5f903-108">Typ</span><span class="sxs-lookup"><span data-stu-id="5f903-108">Type</span></span>|<span data-ttu-id="5f903-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5f903-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f903-110">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="5f903-110">ipAddressOrFQDN</span></span>|<span data-ttu-id="5f903-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5f903-111">String</span></span>|<span data-ttu-id="5f903-112">Die IP-Adresse oder der FQDN</span><span class="sxs-lookup"><span data-stu-id="5f903-112">The IP address or FQDN</span></span>|
|<span data-ttu-id="5f903-113">Proxy</span><span class="sxs-lookup"><span data-stu-id="5f903-113">proxy</span></span>|<span data-ttu-id="5f903-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5f903-114">String</span></span>|<span data-ttu-id="5f903-115">Proxy-IP oder FQDN</span><span class="sxs-lookup"><span data-stu-id="5f903-115">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f903-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5f903-116">Relationships</span></span>
<span data-ttu-id="5f903-117">Keine</span><span class="sxs-lookup"><span data-stu-id="5f903-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f903-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5f903-118">JSON Representation</span></span>
<span data-ttu-id="5f903-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5f903-119">Here is a JSON representation of the resource.</span></span>
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



