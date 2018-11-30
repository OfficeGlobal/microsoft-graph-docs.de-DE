---
title: mediaContentRatingUnitedKingdom-Ressourcentyp
description: Noch nicht dokumentiert
ms.openlocfilehash: 34117db449f65943d0f6e5e0700bbb2c0d19c426
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058608"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="b7d32-103">mediaContentRatingUnitedKingdom-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b7d32-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="b7d32-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b7d32-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7d32-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b7d32-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b7d32-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b7d32-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b7d32-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="b7d32-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="b7d32-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b7d32-108">Properties</span></span>
|<span data-ttu-id="b7d32-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b7d32-109">Property</span></span>|<span data-ttu-id="b7d32-110">Typ</span><span class="sxs-lookup"><span data-stu-id="b7d32-110">Type</span></span>|<span data-ttu-id="b7d32-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b7d32-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7d32-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="b7d32-112">movieRating</span></span>|[<span data-ttu-id="b7d32-113">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="b7d32-113">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="b7d32-114">Bewertung für Großbritannien ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="b7d32-114">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="b7d32-115">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="b7d32-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="b7d32-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="b7d32-116">tvRating</span></span>|[<span data-ttu-id="b7d32-117">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="b7d32-117">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="b7d32-118">TV-Bewertung für Großbritannien ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="b7d32-118">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="b7d32-119">Mögliche Werte sind: `allAllowed`, `allBlocked` und `caution`.</span><span class="sxs-lookup"><span data-stu-id="b7d32-119">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7d32-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b7d32-120">Relationships</span></span>
<span data-ttu-id="b7d32-121">Keine</span><span class="sxs-lookup"><span data-stu-id="b7d32-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b7d32-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b7d32-122">JSON Representation</span></span>
<span data-ttu-id="b7d32-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b7d32-123">Here is a JSON representation of the resource.</span></span>
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





