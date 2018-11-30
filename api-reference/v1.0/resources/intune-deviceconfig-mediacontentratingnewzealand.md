---
title: mediaContentRatingNewZealand-Ressourcentyp
description: Noch nicht dokumentiert
ms.openlocfilehash: 0d34843ef7cc624b222694cc8fbe0fa7a7c1b74c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017815"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="130da-103">mediaContentRatingNewZealand-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="130da-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="130da-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="130da-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="130da-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="130da-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="130da-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="130da-106">Properties</span></span>
|<span data-ttu-id="130da-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="130da-107">Property</span></span>|<span data-ttu-id="130da-108">Typ</span><span class="sxs-lookup"><span data-stu-id="130da-108">Type</span></span>|<span data-ttu-id="130da-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="130da-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="130da-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="130da-110">movieRating</span></span>|[<span data-ttu-id="130da-111">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="130da-111">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="130da-112">Bewertung für Neuseeland ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="130da-112">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="130da-113">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="130da-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="130da-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="130da-114">tvRating</span></span>|[<span data-ttu-id="130da-115">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="130da-115">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="130da-116">TV-Bewertung für Neuseeland ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="130da-116">TV rating selected for New Zealand.</span></span> <span data-ttu-id="130da-117">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance` und `adults`.</span><span class="sxs-lookup"><span data-stu-id="130da-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="130da-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="130da-118">Relationships</span></span>
<span data-ttu-id="130da-119">Keine</span><span class="sxs-lookup"><span data-stu-id="130da-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="130da-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="130da-120">JSON Representation</span></span>
<span data-ttu-id="130da-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="130da-121">Here is a JSON representation of the resource.</span></span>
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



