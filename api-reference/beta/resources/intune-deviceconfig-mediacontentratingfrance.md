---
title: mediaContentRatingFrance-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7aa3c16df6b32f5c5c50f53959aaccc767b39bbd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928143"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="8e409-103">mediaContentRatingFrance-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8e409-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="8e409-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8e409-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e409-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8e409-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8e409-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8e409-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e409-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="8e409-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="8e409-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8e409-108">Properties</span></span>
|<span data-ttu-id="8e409-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8e409-109">Property</span></span>|<span data-ttu-id="8e409-110">Typ</span><span class="sxs-lookup"><span data-stu-id="8e409-110">Type</span></span>|<span data-ttu-id="8e409-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8e409-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e409-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="8e409-112">movieRating</span></span>|[<span data-ttu-id="8e409-113">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="8e409-113">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="8e409-114">Bewertung für Frankreich ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="8e409-114">Movies rating selected for France.</span></span> <span data-ttu-id="8e409-115">Mögliche Werte sind: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="8e409-115">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="8e409-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="8e409-116">tvRating</span></span>|[<span data-ttu-id="8e409-117">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="8e409-117">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="8e409-118">TV-Bewertung für Frankreich ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="8e409-118">TV rating selected for France.</span></span> <span data-ttu-id="8e409-119">Mögliche Werte sind: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="8e409-119">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e409-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8e409-120">Relationships</span></span>
<span data-ttu-id="8e409-121">Keine</span><span class="sxs-lookup"><span data-stu-id="8e409-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8e409-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8e409-122">JSON Representation</span></span>
<span data-ttu-id="8e409-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8e409-123">Here is a JSON representation of the resource.</span></span>
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





