---
title: mediaContentRatingFrance-Ressourcentyp
description: Noch nicht dokumentiert
ms.openlocfilehash: bd2f4933ea05c7db193d700799cdcbdc79490356
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016636"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="bc738-103">mediaContentRatingFrance-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bc738-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="bc738-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bc738-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bc738-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="bc738-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="bc738-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bc738-106">Properties</span></span>
|<span data-ttu-id="bc738-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bc738-107">Property</span></span>|<span data-ttu-id="bc738-108">Typ</span><span class="sxs-lookup"><span data-stu-id="bc738-108">Type</span></span>|<span data-ttu-id="bc738-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc738-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc738-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="bc738-110">movieRating</span></span>|[<span data-ttu-id="bc738-111">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="bc738-111">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="bc738-112">Bewertung für Frankreich ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="bc738-112">Movies rating selected for France.</span></span> <span data-ttu-id="bc738-113">Mögliche Werte sind: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="bc738-113">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="bc738-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="bc738-114">tvRating</span></span>|[<span data-ttu-id="bc738-115">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="bc738-115">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="bc738-116">TV-Bewertung für Frankreich ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="bc738-116">TV rating selected for France.</span></span> <span data-ttu-id="bc738-117">Mögliche Werte sind: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="bc738-117">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc738-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bc738-118">Relationships</span></span>
<span data-ttu-id="bc738-119">Keine</span><span class="sxs-lookup"><span data-stu-id="bc738-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bc738-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bc738-120">JSON Representation</span></span>
<span data-ttu-id="bc738-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bc738-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```



