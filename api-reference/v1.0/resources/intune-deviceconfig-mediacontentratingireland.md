---
title: mediaContentRatingIreland-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 531768883b88e8fc89fe00c1df7a8a9e8767a408
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934877"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="93dd7-103">mediaContentRatingIreland-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="93dd7-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="93dd7-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="93dd7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="93dd7-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="93dd7-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="93dd7-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="93dd7-106">Properties</span></span>
|<span data-ttu-id="93dd7-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="93dd7-107">Property</span></span>|<span data-ttu-id="93dd7-108">Typ</span><span class="sxs-lookup"><span data-stu-id="93dd7-108">Type</span></span>|<span data-ttu-id="93dd7-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="93dd7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93dd7-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="93dd7-110">movieRating</span></span>|[<span data-ttu-id="93dd7-111">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="93dd7-111">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="93dd7-112">Bewertung für Irland ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="93dd7-112">Movies rating selected for Ireland.</span></span> <span data-ttu-id="93dd7-113">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16` und `adults`.</span><span class="sxs-lookup"><span data-stu-id="93dd7-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="93dd7-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="93dd7-114">tvRating</span></span>|[<span data-ttu-id="93dd7-115">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="93dd7-115">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="93dd7-116">TV-Bewertung für Irland ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="93dd7-116">TV rating selected for Ireland.</span></span> <span data-ttu-id="93dd7-117">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="93dd7-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="93dd7-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="93dd7-118">Relationships</span></span>
<span data-ttu-id="93dd7-119">Keine</span><span class="sxs-lookup"><span data-stu-id="93dd7-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="93dd7-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="93dd7-120">JSON Representation</span></span>
<span data-ttu-id="93dd7-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="93dd7-121">Here is a JSON representation of the resource.</span></span>
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



