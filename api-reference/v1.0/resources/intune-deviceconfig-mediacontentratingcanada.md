---
title: mediaContentRatingCanada-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c40691556e9a8f674256c040a98f22e6ef9d717f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857309"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="71cdf-103">mediaContentRatingCanada-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="71cdf-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="71cdf-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="71cdf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71cdf-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="71cdf-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="71cdf-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="71cdf-106">Properties</span></span>
|<span data-ttu-id="71cdf-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="71cdf-107">Property</span></span>|<span data-ttu-id="71cdf-108">Typ</span><span class="sxs-lookup"><span data-stu-id="71cdf-108">Type</span></span>|<span data-ttu-id="71cdf-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71cdf-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71cdf-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="71cdf-110">movieRating</span></span>|[<span data-ttu-id="71cdf-111">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="71cdf-111">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="71cdf-112">Bewertung für Kanada ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="71cdf-112">Movies rating selected for Canada.</span></span> <span data-ttu-id="71cdf-113">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18` und `restricted`.</span><span class="sxs-lookup"><span data-stu-id="71cdf-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="71cdf-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="71cdf-114">tvRating</span></span>|[<span data-ttu-id="71cdf-115">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="71cdf-115">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="71cdf-116">TV-Bewertung für Kanada ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="71cdf-116">TV rating selected for Canada.</span></span> <span data-ttu-id="71cdf-117">Mögliche Werte: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="71cdf-117">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71cdf-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="71cdf-118">Relationships</span></span>
<span data-ttu-id="71cdf-119">Keine</span><span class="sxs-lookup"><span data-stu-id="71cdf-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="71cdf-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="71cdf-120">JSON Representation</span></span>
<span data-ttu-id="71cdf-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="71cdf-121">Here is a JSON representation of the resource.</span></span>
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



