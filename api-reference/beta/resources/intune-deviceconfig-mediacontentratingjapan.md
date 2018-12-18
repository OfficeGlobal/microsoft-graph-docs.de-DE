---
title: mediaContentRatingJapan-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: 98af9a6678b26c2cef15950cae769f3057009479
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337429"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="b229e-103">mediaContentRatingJapan-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b229e-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="b229e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b229e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b229e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b229e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b229e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b229e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b229e-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="b229e-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="b229e-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b229e-108">Properties</span></span>
|<span data-ttu-id="b229e-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b229e-109">Property</span></span>|<span data-ttu-id="b229e-110">Typ</span><span class="sxs-lookup"><span data-stu-id="b229e-110">Type</span></span>|<span data-ttu-id="b229e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b229e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b229e-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="b229e-112">movieRating</span></span>|[<span data-ttu-id="b229e-113">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="b229e-113">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="b229e-114">Bewertung für Japan ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="b229e-114">Movies rating selected for Japan.</span></span> <span data-ttu-id="b229e-115">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="b229e-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="b229e-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="b229e-116">tvRating</span></span>|[<span data-ttu-id="b229e-117">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="b229e-117">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="b229e-118">TV-Bewertung für Japan ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="b229e-118">TV rating selected for Japan.</span></span> <span data-ttu-id="b229e-119">Mögliche Werte sind: `allAllowed`, `allBlocked` und `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="b229e-119">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b229e-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b229e-120">Relationships</span></span>
<span data-ttu-id="b229e-121">Keine</span><span class="sxs-lookup"><span data-stu-id="b229e-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b229e-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b229e-122">JSON Representation</span></span>
<span data-ttu-id="b229e-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b229e-123">Here is a JSON representation of the resource.</span></span>
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





