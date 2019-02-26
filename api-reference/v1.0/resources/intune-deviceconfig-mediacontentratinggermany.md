---
title: mediaContentRatingGermany-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e3c59bf110c55492db49a81a557cef0b421e328
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260354"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="ef44e-103">mediaContentRatingGermany-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ef44e-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="ef44e-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ef44e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef44e-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="ef44e-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="ef44e-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ef44e-106">Properties</span></span>
|<span data-ttu-id="ef44e-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ef44e-107">Property</span></span>|<span data-ttu-id="ef44e-108">Typ</span><span class="sxs-lookup"><span data-stu-id="ef44e-108">Type</span></span>|<span data-ttu-id="ef44e-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ef44e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef44e-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="ef44e-110">movieRating</span></span>|[<span data-ttu-id="ef44e-111">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="ef44e-111">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="ef44e-112">Film Bewertung für Deutschland ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="ef44e-112">Movies rating selected for Germany.</span></span> <span data-ttu-id="ef44e-113">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16` und `adults`.</span><span class="sxs-lookup"><span data-stu-id="ef44e-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="ef44e-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="ef44e-114">tvRating</span></span>|[<span data-ttu-id="ef44e-115">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="ef44e-115">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="ef44e-116">TV-Bewertung für Deutschland ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="ef44e-116">TV rating selected for Germany.</span></span> <span data-ttu-id="ef44e-117">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="ef44e-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ef44e-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ef44e-118">Relationships</span></span>
<span data-ttu-id="ef44e-119">Keine</span><span class="sxs-lookup"><span data-stu-id="ef44e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ef44e-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ef44e-120">JSON Representation</span></span>
<span data-ttu-id="ef44e-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ef44e-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```



