---
title: mediaContentRatingIreland-Ressourcentyp
description: Noch nicht dokumentiert
ms.openlocfilehash: b4348e6f73730d59e6e67b3e102b9ad9caa98add
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016338"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="65f8c-103">mediaContentRatingIreland-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="65f8c-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="65f8c-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="65f8c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65f8c-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="65f8c-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="65f8c-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="65f8c-106">Properties</span></span>
|<span data-ttu-id="65f8c-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="65f8c-107">Property</span></span>|<span data-ttu-id="65f8c-108">Typ</span><span class="sxs-lookup"><span data-stu-id="65f8c-108">Type</span></span>|<span data-ttu-id="65f8c-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65f8c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65f8c-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="65f8c-110">movieRating</span></span>|[<span data-ttu-id="65f8c-111">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="65f8c-111">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="65f8c-112">Bewertung für Irland ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="65f8c-112">Movies rating selected for Ireland.</span></span> <span data-ttu-id="65f8c-113">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16` und `adults`.</span><span class="sxs-lookup"><span data-stu-id="65f8c-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="65f8c-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="65f8c-114">tvRating</span></span>|[<span data-ttu-id="65f8c-115">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="65f8c-115">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="65f8c-116">TV-Bewertung für Irland ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="65f8c-116">TV rating selected for Ireland.</span></span> <span data-ttu-id="65f8c-117">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="65f8c-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65f8c-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="65f8c-118">Relationships</span></span>
<span data-ttu-id="65f8c-119">Keine</span><span class="sxs-lookup"><span data-stu-id="65f8c-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="65f8c-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="65f8c-120">JSON Representation</span></span>
<span data-ttu-id="65f8c-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="65f8c-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingIreland"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingIreland",
  "movieRating": "String",
  "tvRating": "String"
}
```



