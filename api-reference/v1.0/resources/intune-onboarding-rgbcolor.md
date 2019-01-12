---
title: rgbColor-Ressourcentyp
description: Farbe in RGB
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fc40b5cc2ffff02bed89847386db6398f76b3953
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967007"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="68063-103">rgbColor-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="68063-103">rgbColor resource type</span></span>

> <span data-ttu-id="68063-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="68063-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="68063-105">Farbe in RGB</span><span class="sxs-lookup"><span data-stu-id="68063-105">Color in RGB.</span></span>
## <a name="properties"></a><span data-ttu-id="68063-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="68063-106">Properties</span></span>
|<span data-ttu-id="68063-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="68063-107">Property</span></span>|<span data-ttu-id="68063-108">Typ</span><span class="sxs-lookup"><span data-stu-id="68063-108">Type</span></span>|<span data-ttu-id="68063-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="68063-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68063-110">r</span><span class="sxs-lookup"><span data-stu-id="68063-110">r</span></span>|<span data-ttu-id="68063-111">Byte</span><span class="sxs-lookup"><span data-stu-id="68063-111">Byte</span></span>|<span data-ttu-id="68063-112">Rotwert</span><span class="sxs-lookup"><span data-stu-id="68063-112">Red value</span></span>|
|<span data-ttu-id="68063-113">g</span><span class="sxs-lookup"><span data-stu-id="68063-113">g</span></span>|<span data-ttu-id="68063-114">Byte</span><span class="sxs-lookup"><span data-stu-id="68063-114">Byte</span></span>|<span data-ttu-id="68063-115">Grünwert</span><span class="sxs-lookup"><span data-stu-id="68063-115">Green value</span></span>|
|<span data-ttu-id="68063-116">b</span><span class="sxs-lookup"><span data-stu-id="68063-116">b</span></span>|<span data-ttu-id="68063-117">Byte</span><span class="sxs-lookup"><span data-stu-id="68063-117">Byte</span></span>|<span data-ttu-id="68063-118">Blauwert</span><span class="sxs-lookup"><span data-stu-id="68063-118">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="68063-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="68063-119">Relationships</span></span>
<span data-ttu-id="68063-120">Keine</span><span class="sxs-lookup"><span data-stu-id="68063-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="68063-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="68063-121">JSON Representation</span></span>
<span data-ttu-id="68063-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="68063-122">Here is a JSON representation of the resource.</span></span>
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



