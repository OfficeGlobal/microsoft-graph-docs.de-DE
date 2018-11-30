---
title: mediaContentRatingAustralia-Ressourcentyp
description: Noch nicht dokumentiert
ms.openlocfilehash: f60df6c4948d0e0208b545a8a25e31ca29247879
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017819"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="943f4-103">mediaContentRatingAustralia-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="943f4-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="943f4-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="943f4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="943f4-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="943f4-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="943f4-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="943f4-106">Properties</span></span>
|<span data-ttu-id="943f4-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="943f4-107">Property</span></span>|<span data-ttu-id="943f4-108">Typ</span><span class="sxs-lookup"><span data-stu-id="943f4-108">Type</span></span>|<span data-ttu-id="943f4-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="943f4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="943f4-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="943f4-110">movieRating</span></span>|[<span data-ttu-id="943f4-111">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="943f4-111">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="943f4-112">Bewertung für Australien ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="943f4-112">Movies rating selected for Australia.</span></span> <span data-ttu-id="943f4-113">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="943f4-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="943f4-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="943f4-114">tvRating</span></span>|[<span data-ttu-id="943f4-115">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="943f4-115">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="943f4-116">TV-Bewertung für Australien ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="943f4-116">TV rating selected for Australia.</span></span> <span data-ttu-id="943f4-117">Mögliche Werte: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="943f4-117">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="943f4-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="943f4-118">Relationships</span></span>
<span data-ttu-id="943f4-119">Keine</span><span class="sxs-lookup"><span data-stu-id="943f4-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="943f4-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="943f4-120">JSON Representation</span></span>
<span data-ttu-id="943f4-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="943f4-121">Here is a JSON representation of the resource.</span></span>
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



