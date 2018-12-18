---
title: mediaContentRatingUnitedKingdom-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: cd4285f3be40961d2368da180c52e16b0ff6ea47
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332564"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="13528-103">mediaContentRatingUnitedKingdom-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="13528-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="13528-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="13528-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13528-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="13528-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="13528-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="13528-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="13528-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="13528-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="13528-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="13528-108">Properties</span></span>
|<span data-ttu-id="13528-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="13528-109">Property</span></span>|<span data-ttu-id="13528-110">Typ</span><span class="sxs-lookup"><span data-stu-id="13528-110">Type</span></span>|<span data-ttu-id="13528-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="13528-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13528-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="13528-112">movieRating</span></span>|[<span data-ttu-id="13528-113">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="13528-113">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="13528-114">Bewertung für Großbritannien ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="13528-114">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="13528-115">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="13528-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="13528-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="13528-116">tvRating</span></span>|[<span data-ttu-id="13528-117">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="13528-117">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="13528-118">TV-Bewertung für Großbritannien ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="13528-118">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="13528-119">Mögliche Werte sind: `allAllowed`, `allBlocked` und `caution`.</span><span class="sxs-lookup"><span data-stu-id="13528-119">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13528-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="13528-120">Relationships</span></span>
<span data-ttu-id="13528-121">Keine</span><span class="sxs-lookup"><span data-stu-id="13528-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="13528-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="13528-122">JSON Representation</span></span>
<span data-ttu-id="13528-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="13528-123">Here is a JSON representation of the resource.</span></span>
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





