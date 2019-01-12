---
title: mediaContentRatingCanada-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9b4151b810fcfbc56c652492fff9fa1f3f841189
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932182"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="a078b-103">mediaContentRatingCanada-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a078b-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="a078b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a078b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a078b-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="a078b-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="a078b-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a078b-106">Properties</span></span>
|<span data-ttu-id="a078b-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a078b-107">Property</span></span>|<span data-ttu-id="a078b-108">Typ</span><span class="sxs-lookup"><span data-stu-id="a078b-108">Type</span></span>|<span data-ttu-id="a078b-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a078b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a078b-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="a078b-110">movieRating</span></span>|[<span data-ttu-id="a078b-111">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="a078b-111">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="a078b-112">Bewertung für Kanada ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="a078b-112">Movies rating selected for Canada.</span></span> <span data-ttu-id="a078b-113">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18` und `restricted`.</span><span class="sxs-lookup"><span data-stu-id="a078b-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="a078b-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="a078b-114">tvRating</span></span>|[<span data-ttu-id="a078b-115">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="a078b-115">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="a078b-116">TV-Bewertung für Kanada ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="a078b-116">TV rating selected for Canada.</span></span> <span data-ttu-id="a078b-117">Mögliche Werte: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="a078b-117">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a078b-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a078b-118">Relationships</span></span>
<span data-ttu-id="a078b-119">Keine</span><span class="sxs-lookup"><span data-stu-id="a078b-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a078b-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a078b-120">JSON Representation</span></span>
<span data-ttu-id="a078b-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a078b-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingCanada"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingCanada",
  "movieRating": "String",
  "tvRating": "String"
}
```



