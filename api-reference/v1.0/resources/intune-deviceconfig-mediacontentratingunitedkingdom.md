---
title: mediaContentRatingUnitedKingdom-Ressourcentyp
description: Noch nicht dokumentiert
ms.openlocfilehash: 8bc3b7cf1de10a6ef5b72feb7e633018766b0397
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017159"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="0f4fb-103">mediaContentRatingUnitedKingdom-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0f4fb-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="0f4fb-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0f4fb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f4fb-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="0f4fb-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="0f4fb-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0f4fb-106">Properties</span></span>
|<span data-ttu-id="0f4fb-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0f4fb-107">Property</span></span>|<span data-ttu-id="0f4fb-108">Typ</span><span class="sxs-lookup"><span data-stu-id="0f4fb-108">Type</span></span>|<span data-ttu-id="0f4fb-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f4fb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f4fb-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="0f4fb-110">movieRating</span></span>|[<span data-ttu-id="0f4fb-111">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="0f4fb-111">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="0f4fb-112">Bewertung für Großbritannien ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="0f4fb-112">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="0f4fb-113">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="0f4fb-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="0f4fb-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="0f4fb-114">tvRating</span></span>|[<span data-ttu-id="0f4fb-115">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="0f4fb-115">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="0f4fb-116">TV-Bewertung für Großbritannien ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="0f4fb-116">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="0f4fb-117">Mögliche Werte sind: `allAllowed`, `allBlocked` und `caution`.</span><span class="sxs-lookup"><span data-stu-id="0f4fb-117">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f4fb-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0f4fb-118">Relationships</span></span>
<span data-ttu-id="0f4fb-119">Keine</span><span class="sxs-lookup"><span data-stu-id="0f4fb-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0f4fb-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0f4fb-120">JSON Representation</span></span>
<span data-ttu-id="0f4fb-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0f4fb-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedKingdom",
  "movieRating": "String",
  "tvRating": "String"
}
```



