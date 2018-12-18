---
title: mediaContentRatingNewZealand-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: 5daba568ee435c32cc0b3d491c1cedcc61294603
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356105"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="ea027-103">mediaContentRatingNewZealand-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ea027-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="ea027-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ea027-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea027-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="ea027-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="ea027-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ea027-106">Properties</span></span>
|<span data-ttu-id="ea027-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ea027-107">Property</span></span>|<span data-ttu-id="ea027-108">Typ</span><span class="sxs-lookup"><span data-stu-id="ea027-108">Type</span></span>|<span data-ttu-id="ea027-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ea027-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea027-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="ea027-110">movieRating</span></span>|[<span data-ttu-id="ea027-111">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="ea027-111">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="ea027-112">Bewertung für Neuseeland ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="ea027-112">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="ea027-113">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="ea027-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="ea027-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="ea027-114">tvRating</span></span>|[<span data-ttu-id="ea027-115">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="ea027-115">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="ea027-116">TV-Bewertung für Neuseeland ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="ea027-116">TV rating selected for New Zealand.</span></span> <span data-ttu-id="ea027-117">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance` und `adults`.</span><span class="sxs-lookup"><span data-stu-id="ea027-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea027-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ea027-118">Relationships</span></span>
<span data-ttu-id="ea027-119">Keine</span><span class="sxs-lookup"><span data-stu-id="ea027-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ea027-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ea027-120">JSON Representation</span></span>
<span data-ttu-id="ea027-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ea027-121">Here is a JSON representation of the resource.</span></span>
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



