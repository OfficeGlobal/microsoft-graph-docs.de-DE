---
title: mediaContentRatingCanada-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: 310d68ea3ee0fa563b9fe413e26bace51251025a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312495"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="c76a3-103">mediaContentRatingCanada-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c76a3-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="c76a3-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c76a3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c76a3-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="c76a3-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="c76a3-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c76a3-106">Properties</span></span>
|<span data-ttu-id="c76a3-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c76a3-107">Property</span></span>|<span data-ttu-id="c76a3-108">Typ</span><span class="sxs-lookup"><span data-stu-id="c76a3-108">Type</span></span>|<span data-ttu-id="c76a3-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c76a3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c76a3-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="c76a3-110">movieRating</span></span>|[<span data-ttu-id="c76a3-111">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="c76a3-111">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="c76a3-112">Bewertung für Kanada ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="c76a3-112">Movies rating selected for Canada.</span></span> <span data-ttu-id="c76a3-113">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18` und `restricted`.</span><span class="sxs-lookup"><span data-stu-id="c76a3-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="c76a3-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="c76a3-114">tvRating</span></span>|[<span data-ttu-id="c76a3-115">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="c76a3-115">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="c76a3-116">TV-Bewertung für Kanada ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="c76a3-116">TV rating selected for Canada.</span></span> <span data-ttu-id="c76a3-117">Mögliche Werte: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="c76a3-117">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c76a3-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c76a3-118">Relationships</span></span>
<span data-ttu-id="c76a3-119">Keine</span><span class="sxs-lookup"><span data-stu-id="c76a3-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c76a3-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c76a3-120">JSON Representation</span></span>
<span data-ttu-id="c76a3-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c76a3-121">Here is a JSON representation of the resource.</span></span>
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



