---
title: iPv4Range-Ressourcentyp
description: Definition des IPv4-Umfangs.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 14cb0d88013b13f57b186f5388d5ac89f60db043
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256840"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="0999f-103">iPv4Range-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0999f-103">iPv4Range resource type</span></span>

> <span data-ttu-id="0999f-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0999f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0999f-105">Definition des IPv4-Umfangs.</span><span class="sxs-lookup"><span data-stu-id="0999f-105">IPv4 Range definition.</span></span>


<span data-ttu-id="0999f-106">Erbt von [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="0999f-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0999f-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0999f-107">Properties</span></span>
|<span data-ttu-id="0999f-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0999f-108">Property</span></span>|<span data-ttu-id="0999f-109">Typ</span><span class="sxs-lookup"><span data-stu-id="0999f-109">Type</span></span>|<span data-ttu-id="0999f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0999f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0999f-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="0999f-111">lowerAddress</span></span>|<span data-ttu-id="0999f-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0999f-112">String</span></span>|<span data-ttu-id="0999f-113">Niedrigere Adresse.</span><span class="sxs-lookup"><span data-stu-id="0999f-113">Lower address.</span></span>|
|<span data-ttu-id="0999f-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="0999f-114">upperAddress</span></span>|<span data-ttu-id="0999f-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0999f-115">String</span></span>|<span data-ttu-id="0999f-116">Obere Adresse.</span><span class="sxs-lookup"><span data-stu-id="0999f-116">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0999f-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0999f-117">Relationships</span></span>
<span data-ttu-id="0999f-118">Keine</span><span class="sxs-lookup"><span data-stu-id="0999f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0999f-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0999f-119">JSON Representation</span></span>
<span data-ttu-id="0999f-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0999f-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv4Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv4Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



