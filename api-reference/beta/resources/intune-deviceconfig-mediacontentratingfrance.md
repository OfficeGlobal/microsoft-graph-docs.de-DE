---
title: mediaContentRatingFrance-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: ef16120633618dfef86906554eaabd9eb41a95e6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312705"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="60728-103">mediaContentRatingFrance-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="60728-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="60728-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="60728-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="60728-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="60728-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="60728-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="60728-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="60728-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="60728-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="60728-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="60728-108">Properties</span></span>
|<span data-ttu-id="60728-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="60728-109">Property</span></span>|<span data-ttu-id="60728-110">Typ</span><span class="sxs-lookup"><span data-stu-id="60728-110">Type</span></span>|<span data-ttu-id="60728-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="60728-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60728-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="60728-112">movieRating</span></span>|[<span data-ttu-id="60728-113">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="60728-113">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="60728-114">Bewertung für Frankreich ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="60728-114">Movies rating selected for France.</span></span> <span data-ttu-id="60728-115">Mögliche Werte sind: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="60728-115">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="60728-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="60728-116">tvRating</span></span>|[<span data-ttu-id="60728-117">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="60728-117">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="60728-118">TV-Bewertung für Frankreich ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="60728-118">TV rating selected for France.</span></span> <span data-ttu-id="60728-119">Mögliche Werte sind: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="60728-119">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60728-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="60728-120">Relationships</span></span>
<span data-ttu-id="60728-121">Keine</span><span class="sxs-lookup"><span data-stu-id="60728-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="60728-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="60728-122">JSON Representation</span></span>
<span data-ttu-id="60728-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="60728-123">Here is a JSON representation of the resource.</span></span>
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





