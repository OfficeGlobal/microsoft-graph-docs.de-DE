---
title: mediaContentRatingJapan-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 202b778fefe1236577f61058025714ea0f337826
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943018"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="fc84e-103">mediaContentRatingJapan-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="fc84e-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="fc84e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fc84e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fc84e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fc84e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fc84e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fc84e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fc84e-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="fc84e-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="fc84e-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fc84e-108">Properties</span></span>
|<span data-ttu-id="fc84e-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fc84e-109">Property</span></span>|<span data-ttu-id="fc84e-110">Typ</span><span class="sxs-lookup"><span data-stu-id="fc84e-110">Type</span></span>|<span data-ttu-id="fc84e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fc84e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc84e-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="fc84e-112">movieRating</span></span>|[<span data-ttu-id="fc84e-113">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="fc84e-113">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="fc84e-114">Bewertung für Japan ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="fc84e-114">Movies rating selected for Japan.</span></span> <span data-ttu-id="fc84e-115">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="fc84e-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="fc84e-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="fc84e-116">tvRating</span></span>|[<span data-ttu-id="fc84e-117">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="fc84e-117">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="fc84e-118">TV-Bewertung für Japan ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="fc84e-118">TV rating selected for Japan.</span></span> <span data-ttu-id="fc84e-119">Mögliche Werte sind: `allAllowed`, `allBlocked` und `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="fc84e-119">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc84e-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fc84e-120">Relationships</span></span>
<span data-ttu-id="fc84e-121">Keine</span><span class="sxs-lookup"><span data-stu-id="fc84e-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fc84e-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fc84e-122">JSON Representation</span></span>
<span data-ttu-id="fc84e-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fc84e-123">Here is a JSON representation of the resource.</span></span>
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





