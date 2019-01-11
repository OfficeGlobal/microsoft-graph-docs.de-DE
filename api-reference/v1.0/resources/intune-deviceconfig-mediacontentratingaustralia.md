---
title: mediaContentRatingAustralia-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0860a17671b2923c2be9b5b469f93d443e808f53
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891483"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="0cfab-103">mediaContentRatingAustralia-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0cfab-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="0cfab-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0cfab-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0cfab-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="0cfab-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="0cfab-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0cfab-106">Properties</span></span>
|<span data-ttu-id="0cfab-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0cfab-107">Property</span></span>|<span data-ttu-id="0cfab-108">Typ</span><span class="sxs-lookup"><span data-stu-id="0cfab-108">Type</span></span>|<span data-ttu-id="0cfab-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0cfab-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cfab-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="0cfab-110">movieRating</span></span>|[<span data-ttu-id="0cfab-111">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="0cfab-111">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="0cfab-112">Bewertung für Australien ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="0cfab-112">Movies rating selected for Australia.</span></span> <span data-ttu-id="0cfab-113">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="0cfab-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="0cfab-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="0cfab-114">tvRating</span></span>|[<span data-ttu-id="0cfab-115">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="0cfab-115">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="0cfab-116">TV-Bewertung für Australien ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="0cfab-116">TV rating selected for Australia.</span></span> <span data-ttu-id="0cfab-117">Mögliche Werte: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="0cfab-117">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0cfab-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0cfab-118">Relationships</span></span>
<span data-ttu-id="0cfab-119">Keine</span><span class="sxs-lookup"><span data-stu-id="0cfab-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0cfab-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0cfab-120">JSON Representation</span></span>
<span data-ttu-id="0cfab-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0cfab-121">Here is a JSON representation of the resource.</span></span>
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



