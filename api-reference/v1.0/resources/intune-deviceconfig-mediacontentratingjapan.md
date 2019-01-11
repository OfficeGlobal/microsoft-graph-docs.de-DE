---
title: mediaContentRatingJapan-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a0f394b85af0fd1f1c85a8db34025b2e1f139521
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822134"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="61d4d-103">mediaContentRatingJapan-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="61d4d-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="61d4d-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="61d4d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61d4d-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="61d4d-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="61d4d-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="61d4d-106">Properties</span></span>
|<span data-ttu-id="61d4d-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="61d4d-107">Property</span></span>|<span data-ttu-id="61d4d-108">Typ</span><span class="sxs-lookup"><span data-stu-id="61d4d-108">Type</span></span>|<span data-ttu-id="61d4d-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61d4d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61d4d-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="61d4d-110">movieRating</span></span>|[<span data-ttu-id="61d4d-111">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="61d4d-111">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="61d4d-112">Bewertung für Japan ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="61d4d-112">Movies rating selected for Japan.</span></span> <span data-ttu-id="61d4d-113">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="61d4d-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="61d4d-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="61d4d-114">tvRating</span></span>|[<span data-ttu-id="61d4d-115">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="61d4d-115">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="61d4d-116">TV-Bewertung für Japan ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="61d4d-116">TV rating selected for Japan.</span></span> <span data-ttu-id="61d4d-117">Mögliche Werte sind: `allAllowed`, `allBlocked` und `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="61d4d-117">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61d4d-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="61d4d-118">Relationships</span></span>
<span data-ttu-id="61d4d-119">Keine</span><span class="sxs-lookup"><span data-stu-id="61d4d-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="61d4d-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="61d4d-120">JSON Representation</span></span>
<span data-ttu-id="61d4d-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="61d4d-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```



