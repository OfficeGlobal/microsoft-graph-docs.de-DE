---
title: mediaContentRatingIreland-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: 6ade4ea9d5f2236803a8515b94ebc57f32ce3cd7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337492"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="5fc37-103">mediaContentRatingIreland-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5fc37-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="5fc37-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5fc37-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5fc37-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5fc37-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5fc37-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5fc37-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5fc37-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="5fc37-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="5fc37-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5fc37-108">Properties</span></span>
|<span data-ttu-id="5fc37-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5fc37-109">Property</span></span>|<span data-ttu-id="5fc37-110">Typ</span><span class="sxs-lookup"><span data-stu-id="5fc37-110">Type</span></span>|<span data-ttu-id="5fc37-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5fc37-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fc37-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="5fc37-112">movieRating</span></span>|[<span data-ttu-id="5fc37-113">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="5fc37-113">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="5fc37-114">Bewertung für Irland ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="5fc37-114">Movies rating selected for Ireland.</span></span> <span data-ttu-id="5fc37-115">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16` und `adults`.</span><span class="sxs-lookup"><span data-stu-id="5fc37-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="5fc37-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="5fc37-116">tvRating</span></span>|[<span data-ttu-id="5fc37-117">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="5fc37-117">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="5fc37-118">TV-Bewertung für Irland ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="5fc37-118">TV rating selected for Ireland.</span></span> <span data-ttu-id="5fc37-119">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="5fc37-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5fc37-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5fc37-120">Relationships</span></span>
<span data-ttu-id="5fc37-121">Keine</span><span class="sxs-lookup"><span data-stu-id="5fc37-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5fc37-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5fc37-122">JSON Representation</span></span>
<span data-ttu-id="5fc37-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5fc37-123">Here is a JSON representation of the resource.</span></span>
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





