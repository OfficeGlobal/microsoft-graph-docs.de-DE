---
title: mediaContentRatingAustralia-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ae1cb934af017c751ae2bcf05cd992668a452ed6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166766"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="78be4-103">mediaContentRatingAustralia-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="78be4-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="78be4-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="78be4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78be4-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="78be4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78be4-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="78be4-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="78be4-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="78be4-107">Properties</span></span>
|<span data-ttu-id="78be4-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="78be4-108">Property</span></span>|<span data-ttu-id="78be4-109">Typ</span><span class="sxs-lookup"><span data-stu-id="78be4-109">Type</span></span>|<span data-ttu-id="78be4-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="78be4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78be4-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="78be4-111">movieRating</span></span>|[<span data-ttu-id="78be4-112">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="78be4-112">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="78be4-113">Film Bewertung für Australien ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="78be4-113">Movies rating selected for Australia.</span></span> <span data-ttu-id="78be4-114">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="78be4-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="78be4-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="78be4-115">tvRating</span></span>|[<span data-ttu-id="78be4-116">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="78be4-116">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="78be4-117">TV-Bewertung für Australien ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="78be4-117">TV rating selected for Australia.</span></span> <span data-ttu-id="78be4-118">Mögliche Werte: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="78be4-118">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78be4-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="78be4-119">Relationships</span></span>
<span data-ttu-id="78be4-120">Keine</span><span class="sxs-lookup"><span data-stu-id="78be4-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="78be4-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="78be4-121">JSON Representation</span></span>
<span data-ttu-id="78be4-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="78be4-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```




