---
title: iPv6Range-Ressourcentyp
description: IPv6-Range-Definition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6b54782b1851ea800b548f02b34f60da3a3236a3
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571536"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="69aa8-103">iPv6Range-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="69aa8-103">iPv6Range resource type</span></span>

> <span data-ttu-id="69aa8-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="69aa8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69aa8-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="69aa8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69aa8-106">IPv6-Range-Definition.</span><span class="sxs-lookup"><span data-stu-id="69aa8-106">IPv6 Range definition.</span></span>


<span data-ttu-id="69aa8-107">Erbt von [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="69aa8-107">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="69aa8-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="69aa8-108">Properties</span></span>
|<span data-ttu-id="69aa8-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="69aa8-109">Property</span></span>|<span data-ttu-id="69aa8-110">Typ</span><span class="sxs-lookup"><span data-stu-id="69aa8-110">Type</span></span>|<span data-ttu-id="69aa8-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="69aa8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69aa8-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="69aa8-112">lowerAddress</span></span>|<span data-ttu-id="69aa8-113">String</span><span class="sxs-lookup"><span data-stu-id="69aa8-113">String</span></span>|<span data-ttu-id="69aa8-114">Niedrigere Adresse.</span><span class="sxs-lookup"><span data-stu-id="69aa8-114">Lower address.</span></span>|
|<span data-ttu-id="69aa8-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="69aa8-115">upperAddress</span></span>|<span data-ttu-id="69aa8-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="69aa8-116">String</span></span>|<span data-ttu-id="69aa8-117">Obere Adresse.</span><span class="sxs-lookup"><span data-stu-id="69aa8-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69aa8-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="69aa8-118">Relationships</span></span>
<span data-ttu-id="69aa8-119">Keine</span><span class="sxs-lookup"><span data-stu-id="69aa8-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="69aa8-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="69aa8-120">JSON Representation</span></span>
<span data-ttu-id="69aa8-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="69aa8-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv6Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv6Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```




