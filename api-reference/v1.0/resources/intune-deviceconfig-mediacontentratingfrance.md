---
title: mediaContentRatingFrance-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4f6fe2e4f4ca0f629ac0d4dbc387aab68122896c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913114"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="e9725-103">mediaContentRatingFrance-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e9725-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="e9725-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e9725-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e9725-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e9725-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="e9725-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e9725-106">Properties</span></span>
|<span data-ttu-id="e9725-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e9725-107">Property</span></span>|<span data-ttu-id="e9725-108">Typ</span><span class="sxs-lookup"><span data-stu-id="e9725-108">Type</span></span>|<span data-ttu-id="e9725-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e9725-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9725-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="e9725-110">movieRating</span></span>|[<span data-ttu-id="e9725-111">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="e9725-111">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="e9725-112">Bewertung für Frankreich ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="e9725-112">Movies rating selected for France.</span></span> <span data-ttu-id="e9725-113">Mögliche Werte sind: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="e9725-113">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="e9725-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="e9725-114">tvRating</span></span>|[<span data-ttu-id="e9725-115">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="e9725-115">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="e9725-116">TV-Bewertung für Frankreich ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="e9725-116">TV rating selected for France.</span></span> <span data-ttu-id="e9725-117">Mögliche Werte sind: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="e9725-117">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9725-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e9725-118">Relationships</span></span>
<span data-ttu-id="e9725-119">Keine</span><span class="sxs-lookup"><span data-stu-id="e9725-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e9725-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e9725-120">JSON Representation</span></span>
<span data-ttu-id="e9725-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e9725-121">Here is a JSON representation of the resource.</span></span>
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



