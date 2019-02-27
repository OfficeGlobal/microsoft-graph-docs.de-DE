---
title: mediaContentRatingCanada-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 88975975b07eb2805ee5f73cc416e3803d5fe24f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253316"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="2192a-103">mediaContentRatingCanada-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2192a-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="2192a-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2192a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2192a-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="2192a-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="2192a-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2192a-106">Properties</span></span>
|<span data-ttu-id="2192a-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2192a-107">Property</span></span>|<span data-ttu-id="2192a-108">Typ</span><span class="sxs-lookup"><span data-stu-id="2192a-108">Type</span></span>|<span data-ttu-id="2192a-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2192a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2192a-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="2192a-110">movieRating</span></span>|[<span data-ttu-id="2192a-111">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="2192a-111">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="2192a-112">Ausgewählte Filme für Kanada.</span><span class="sxs-lookup"><span data-stu-id="2192a-112">Movies rating selected for Canada.</span></span> <span data-ttu-id="2192a-113">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18` und `restricted`.</span><span class="sxs-lookup"><span data-stu-id="2192a-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="2192a-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="2192a-114">tvRating</span></span>|[<span data-ttu-id="2192a-115">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="2192a-115">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="2192a-116">TV-Bewertung für Kanada ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="2192a-116">TV rating selected for Canada.</span></span> <span data-ttu-id="2192a-117">Mögliche Werte: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="2192a-117">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2192a-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2192a-118">Relationships</span></span>
<span data-ttu-id="2192a-119">Keine</span><span class="sxs-lookup"><span data-stu-id="2192a-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2192a-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2192a-120">JSON Representation</span></span>
<span data-ttu-id="2192a-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2192a-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingCanada"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingCanada",
  "movieRating": "String",
  "tvRating": "String"
}
```



