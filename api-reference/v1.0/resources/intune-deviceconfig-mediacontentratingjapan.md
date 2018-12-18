---
title: mediaContentRatingJapan-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: 1913b28b3020ffdc51edea1a8d93dd726d70efdd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328469"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="56e26-103">mediaContentRatingJapan-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="56e26-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="56e26-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="56e26-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56e26-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="56e26-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="56e26-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="56e26-106">Properties</span></span>
|<span data-ttu-id="56e26-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="56e26-107">Property</span></span>|<span data-ttu-id="56e26-108">Typ</span><span class="sxs-lookup"><span data-stu-id="56e26-108">Type</span></span>|<span data-ttu-id="56e26-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="56e26-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56e26-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="56e26-110">movieRating</span></span>|[<span data-ttu-id="56e26-111">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="56e26-111">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="56e26-112">Bewertung für Japan ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="56e26-112">Movies rating selected for Japan.</span></span> <span data-ttu-id="56e26-113">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="56e26-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="56e26-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="56e26-114">tvRating</span></span>|[<span data-ttu-id="56e26-115">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="56e26-115">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="56e26-116">TV-Bewertung für Japan ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="56e26-116">TV rating selected for Japan.</span></span> <span data-ttu-id="56e26-117">Mögliche Werte sind: `allAllowed`, `allBlocked` und `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="56e26-117">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="56e26-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="56e26-118">Relationships</span></span>
<span data-ttu-id="56e26-119">Keine</span><span class="sxs-lookup"><span data-stu-id="56e26-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="56e26-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="56e26-120">JSON Representation</span></span>
<span data-ttu-id="56e26-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="56e26-121">Here is a JSON representation of the resource.</span></span>
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



