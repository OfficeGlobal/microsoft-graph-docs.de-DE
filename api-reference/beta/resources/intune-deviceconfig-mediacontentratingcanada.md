---
title: mediaContentRatingCanada-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 38f3bac4e8410a3c63bd07319888ab0a5fc7df19
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146347"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="66a5d-103">mediaContentRatingCanada-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="66a5d-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="66a5d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="66a5d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66a5d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="66a5d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66a5d-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="66a5d-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="66a5d-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="66a5d-107">Properties</span></span>
|<span data-ttu-id="66a5d-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="66a5d-108">Property</span></span>|<span data-ttu-id="66a5d-109">Typ</span><span class="sxs-lookup"><span data-stu-id="66a5d-109">Type</span></span>|<span data-ttu-id="66a5d-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="66a5d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66a5d-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="66a5d-111">movieRating</span></span>|[<span data-ttu-id="66a5d-112">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="66a5d-112">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="66a5d-113">Ausgewählte Filme für Kanada.</span><span class="sxs-lookup"><span data-stu-id="66a5d-113">Movies rating selected for Canada.</span></span> <span data-ttu-id="66a5d-114">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18` und `restricted`.</span><span class="sxs-lookup"><span data-stu-id="66a5d-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="66a5d-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="66a5d-115">tvRating</span></span>|[<span data-ttu-id="66a5d-116">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="66a5d-116">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="66a5d-117">TV-Bewertung für Kanada ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="66a5d-117">TV rating selected for Canada.</span></span> <span data-ttu-id="66a5d-118">Mögliche Werte: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="66a5d-118">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66a5d-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="66a5d-119">Relationships</span></span>
<span data-ttu-id="66a5d-120">Keine</span><span class="sxs-lookup"><span data-stu-id="66a5d-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="66a5d-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="66a5d-121">JSON Representation</span></span>
<span data-ttu-id="66a5d-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="66a5d-122">Here is a JSON representation of the resource.</span></span>
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




