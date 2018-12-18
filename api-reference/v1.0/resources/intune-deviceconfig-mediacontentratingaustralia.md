---
title: mediaContentRatingAustralia-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: 01d809b43bc8ce68ffc92600d3634c8bd437a954
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319502"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="d6327-103">mediaContentRatingAustralia-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d6327-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="d6327-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d6327-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6327-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="d6327-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="d6327-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d6327-106">Properties</span></span>
|<span data-ttu-id="d6327-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d6327-107">Property</span></span>|<span data-ttu-id="d6327-108">Typ</span><span class="sxs-lookup"><span data-stu-id="d6327-108">Type</span></span>|<span data-ttu-id="d6327-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d6327-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6327-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="d6327-110">movieRating</span></span>|[<span data-ttu-id="d6327-111">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="d6327-111">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="d6327-112">Bewertung für Australien ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="d6327-112">Movies rating selected for Australia.</span></span> <span data-ttu-id="d6327-113">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="d6327-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="d6327-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="d6327-114">tvRating</span></span>|[<span data-ttu-id="d6327-115">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="d6327-115">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="d6327-116">TV-Bewertung für Australien ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="d6327-116">TV rating selected for Australia.</span></span> <span data-ttu-id="d6327-117">Mögliche Werte: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="d6327-117">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6327-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d6327-118">Relationships</span></span>
<span data-ttu-id="d6327-119">Keine</span><span class="sxs-lookup"><span data-stu-id="d6327-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d6327-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d6327-120">JSON Representation</span></span>
<span data-ttu-id="d6327-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d6327-121">Here is a JSON representation of the resource.</span></span>
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



