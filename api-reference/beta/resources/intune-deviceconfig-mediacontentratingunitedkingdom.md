---
title: mediaContentRatingUnitedKingdom-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e4ab6731bc486918815efe0d3f4c7f6f2638329d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953301"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="01197-103">mediaContentRatingUnitedKingdom-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="01197-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="01197-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="01197-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01197-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="01197-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="01197-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="01197-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="01197-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="01197-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="01197-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="01197-108">Properties</span></span>
|<span data-ttu-id="01197-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="01197-109">Property</span></span>|<span data-ttu-id="01197-110">Typ</span><span class="sxs-lookup"><span data-stu-id="01197-110">Type</span></span>|<span data-ttu-id="01197-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="01197-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01197-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="01197-112">movieRating</span></span>|[<span data-ttu-id="01197-113">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="01197-113">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="01197-114">Bewertung für Großbritannien ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="01197-114">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="01197-115">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="01197-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="01197-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="01197-116">tvRating</span></span>|[<span data-ttu-id="01197-117">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="01197-117">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="01197-118">TV-Bewertung für Großbritannien ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="01197-118">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="01197-119">Mögliche Werte sind: `allAllowed`, `allBlocked` und `caution`.</span><span class="sxs-lookup"><span data-stu-id="01197-119">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="01197-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="01197-120">Relationships</span></span>
<span data-ttu-id="01197-121">Keine</span><span class="sxs-lookup"><span data-stu-id="01197-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="01197-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="01197-122">JSON Representation</span></span>
<span data-ttu-id="01197-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="01197-123">Here is a JSON representation of the resource.</span></span>
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





