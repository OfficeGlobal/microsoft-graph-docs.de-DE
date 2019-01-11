---
title: mediaContentRatingJapan-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8877e1b5f2c6031725c07a02b387da4ce5bc9136
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856528"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="647ff-103">mediaContentRatingJapan-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="647ff-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="647ff-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="647ff-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="647ff-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="647ff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="647ff-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="647ff-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="647ff-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="647ff-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="647ff-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="647ff-108">Properties</span></span>
|<span data-ttu-id="647ff-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="647ff-109">Property</span></span>|<span data-ttu-id="647ff-110">Typ</span><span class="sxs-lookup"><span data-stu-id="647ff-110">Type</span></span>|<span data-ttu-id="647ff-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="647ff-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="647ff-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="647ff-112">movieRating</span></span>|[<span data-ttu-id="647ff-113">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="647ff-113">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="647ff-114">Bewertung für Japan ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="647ff-114">Movies rating selected for Japan.</span></span> <span data-ttu-id="647ff-115">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="647ff-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="647ff-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="647ff-116">tvRating</span></span>|[<span data-ttu-id="647ff-117">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="647ff-117">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="647ff-118">TV-Bewertung für Japan ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="647ff-118">TV rating selected for Japan.</span></span> <span data-ttu-id="647ff-119">Mögliche Werte sind: `allAllowed`, `allBlocked` und `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="647ff-119">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="647ff-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="647ff-120">Relationships</span></span>
<span data-ttu-id="647ff-121">Keine</span><span class="sxs-lookup"><span data-stu-id="647ff-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="647ff-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="647ff-122">JSON Representation</span></span>
<span data-ttu-id="647ff-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="647ff-123">Here is a JSON representation of the resource.</span></span>
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





