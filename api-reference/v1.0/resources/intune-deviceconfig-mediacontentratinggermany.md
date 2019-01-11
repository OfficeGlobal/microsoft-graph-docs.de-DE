---
title: mediaContentRatingGermany-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5dd25a8bd29211fd593daf3ecea20a7808384bc1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860004"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="acad3-103">mediaContentRatingGermany-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="acad3-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="acad3-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="acad3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="acad3-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="acad3-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="acad3-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="acad3-106">Properties</span></span>
|<span data-ttu-id="acad3-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="acad3-107">Property</span></span>|<span data-ttu-id="acad3-108">Typ</span><span class="sxs-lookup"><span data-stu-id="acad3-108">Type</span></span>|<span data-ttu-id="acad3-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="acad3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acad3-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="acad3-110">movieRating</span></span>|[<span data-ttu-id="acad3-111">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="acad3-111">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="acad3-112">Bewertung für Deutschland ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="acad3-112">Movies rating selected for Germany.</span></span> <span data-ttu-id="acad3-113">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16` und `adults`.</span><span class="sxs-lookup"><span data-stu-id="acad3-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="acad3-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="acad3-114">tvRating</span></span>|[<span data-ttu-id="acad3-115">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="acad3-115">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="acad3-116">TV-Bewertung für Deutschland ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="acad3-116">TV rating selected for Germany.</span></span> <span data-ttu-id="acad3-117">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="acad3-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="acad3-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="acad3-118">Relationships</span></span>
<span data-ttu-id="acad3-119">Keine</span><span class="sxs-lookup"><span data-stu-id="acad3-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="acad3-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="acad3-120">JSON Representation</span></span>
<span data-ttu-id="acad3-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="acad3-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```



