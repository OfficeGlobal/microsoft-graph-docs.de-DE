---
title: mediaContentRatingJapan-Ressourcentyp
description: Noch nicht dokumentiert
ms.openlocfilehash: 15e905355133545db2cdf0864fcbba7e9c226183
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017395"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="f8780-103">mediaContentRatingJapan-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f8780-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="f8780-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f8780-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8780-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="f8780-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="f8780-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f8780-106">Properties</span></span>
|<span data-ttu-id="f8780-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f8780-107">Property</span></span>|<span data-ttu-id="f8780-108">Typ</span><span class="sxs-lookup"><span data-stu-id="f8780-108">Type</span></span>|<span data-ttu-id="f8780-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8780-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8780-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="f8780-110">movieRating</span></span>|[<span data-ttu-id="f8780-111">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="f8780-111">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="f8780-112">Bewertung für Japan ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="f8780-112">Movies rating selected for Japan.</span></span> <span data-ttu-id="f8780-113">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="f8780-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="f8780-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="f8780-114">tvRating</span></span>|[<span data-ttu-id="f8780-115">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="f8780-115">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="f8780-116">TV-Bewertung für Japan ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="f8780-116">TV rating selected for Japan.</span></span> <span data-ttu-id="f8780-117">Mögliche Werte sind: `allAllowed`, `allBlocked` und `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="f8780-117">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8780-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f8780-118">Relationships</span></span>
<span data-ttu-id="f8780-119">Keine</span><span class="sxs-lookup"><span data-stu-id="f8780-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f8780-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f8780-120">JSON Representation</span></span>
<span data-ttu-id="f8780-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f8780-121">Here is a JSON representation of the resource.</span></span>
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



