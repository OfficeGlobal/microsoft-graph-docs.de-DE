---
title: mediaContentRatingNewZealand-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5d4a22f9510a615dab746912aed1de5123184ca3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850547"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="412e8-103">mediaContentRatingNewZealand-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="412e8-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="412e8-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="412e8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="412e8-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="412e8-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="412e8-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="412e8-106">Properties</span></span>
|<span data-ttu-id="412e8-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="412e8-107">Property</span></span>|<span data-ttu-id="412e8-108">Typ</span><span class="sxs-lookup"><span data-stu-id="412e8-108">Type</span></span>|<span data-ttu-id="412e8-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="412e8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="412e8-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="412e8-110">movieRating</span></span>|[<span data-ttu-id="412e8-111">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="412e8-111">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="412e8-112">Bewertung für Neuseeland ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="412e8-112">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="412e8-113">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="412e8-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="412e8-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="412e8-114">tvRating</span></span>|[<span data-ttu-id="412e8-115">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="412e8-115">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="412e8-116">TV-Bewertung für Neuseeland ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="412e8-116">TV rating selected for New Zealand.</span></span> <span data-ttu-id="412e8-117">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance` und `adults`.</span><span class="sxs-lookup"><span data-stu-id="412e8-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="412e8-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="412e8-118">Relationships</span></span>
<span data-ttu-id="412e8-119">Keine</span><span class="sxs-lookup"><span data-stu-id="412e8-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="412e8-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="412e8-120">JSON Representation</span></span>
<span data-ttu-id="412e8-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="412e8-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```



