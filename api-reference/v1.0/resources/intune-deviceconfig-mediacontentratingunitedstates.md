---
title: mediaContentRatingUnitedStates-Ressourcentyp
description: Noch nicht dokumentiert
ms.openlocfilehash: b96241f31e232f39f62a09d7fff8560e5a89e237
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019006"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="55049-103">mediaContentRatingUnitedStates-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="55049-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="55049-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="55049-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="55049-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="55049-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="55049-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="55049-106">Properties</span></span>
|<span data-ttu-id="55049-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="55049-107">Property</span></span>|<span data-ttu-id="55049-108">Typ</span><span class="sxs-lookup"><span data-stu-id="55049-108">Type</span></span>|<span data-ttu-id="55049-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="55049-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55049-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="55049-110">movieRating</span></span>|[<span data-ttu-id="55049-111">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="55049-111">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="55049-112">Bewertung für USA ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="55049-112">Movies rating selected for United States.</span></span> <span data-ttu-id="55049-113">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted` und `adults`.</span><span class="sxs-lookup"><span data-stu-id="55049-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="55049-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="55049-114">tvRating</span></span>|[<span data-ttu-id="55049-115">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="55049-115">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="55049-116">TV-Bewertung für die USA ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="55049-116">TV rating selected for United States.</span></span> <span data-ttu-id="55049-117">Mögliche Werte: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="55049-117">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55049-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="55049-118">Relationships</span></span>
<span data-ttu-id="55049-119">Keine</span><span class="sxs-lookup"><span data-stu-id="55049-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="55049-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="55049-120">JSON Representation</span></span>
<span data-ttu-id="55049-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="55049-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedStates",
  "movieRating": "String",
  "tvRating": "String"
}
```



