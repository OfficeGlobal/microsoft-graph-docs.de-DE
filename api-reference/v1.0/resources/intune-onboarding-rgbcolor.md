---
title: rgbColor-Ressourcentyp
description: Farbe in RGB
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9d2222d7142ea033a8db2c2ce263da04c3b33153
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250299"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="6b7e8-103">rgbColor-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6b7e8-103">rgbColor resource type</span></span>

> <span data-ttu-id="6b7e8-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6b7e8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b7e8-105">Farbe in RGB</span><span class="sxs-lookup"><span data-stu-id="6b7e8-105">Color in RGB.</span></span>

## <a name="properties"></a><span data-ttu-id="6b7e8-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6b7e8-106">Properties</span></span>
|<span data-ttu-id="6b7e8-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6b7e8-107">Property</span></span>|<span data-ttu-id="6b7e8-108">Typ</span><span class="sxs-lookup"><span data-stu-id="6b7e8-108">Type</span></span>|<span data-ttu-id="6b7e8-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6b7e8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b7e8-110">r</span><span class="sxs-lookup"><span data-stu-id="6b7e8-110">r</span></span>|<span data-ttu-id="6b7e8-111">Byte</span><span class="sxs-lookup"><span data-stu-id="6b7e8-111">Byte</span></span>|<span data-ttu-id="6b7e8-112">Rotwert</span><span class="sxs-lookup"><span data-stu-id="6b7e8-112">Red value</span></span>|
|<span data-ttu-id="6b7e8-113">g</span><span class="sxs-lookup"><span data-stu-id="6b7e8-113">g</span></span>|<span data-ttu-id="6b7e8-114">Byte</span><span class="sxs-lookup"><span data-stu-id="6b7e8-114">Byte</span></span>|<span data-ttu-id="6b7e8-115">Grünwert</span><span class="sxs-lookup"><span data-stu-id="6b7e8-115">Green value</span></span>|
|<span data-ttu-id="6b7e8-116">b</span><span class="sxs-lookup"><span data-stu-id="6b7e8-116">b</span></span>|<span data-ttu-id="6b7e8-117">Byte</span><span class="sxs-lookup"><span data-stu-id="6b7e8-117">Byte</span></span>|<span data-ttu-id="6b7e8-118">Blauwert</span><span class="sxs-lookup"><span data-stu-id="6b7e8-118">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b7e8-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6b7e8-119">Relationships</span></span>
<span data-ttu-id="6b7e8-120">Keine</span><span class="sxs-lookup"><span data-stu-id="6b7e8-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b7e8-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6b7e8-121">JSON Representation</span></span>
<span data-ttu-id="6b7e8-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6b7e8-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rgbColor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rgbColor",
  "r": 1024,
  "g": 1024,
  "b": 1024
}
```



