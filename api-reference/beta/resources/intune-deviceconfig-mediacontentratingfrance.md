---
title: mediaContentRatingFrance-Ressourcentyp
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bb199abfc350a8b88913e353d377745714368c95
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412366"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="4b7e5-103">mediaContentRatingFrance-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4b7e5-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="4b7e5-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="4b7e5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4b7e5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4b7e5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4b7e5-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4b7e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b7e5-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="4b7e5-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="4b7e5-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4b7e5-108">Properties</span></span>
|<span data-ttu-id="4b7e5-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4b7e5-109">Property</span></span>|<span data-ttu-id="4b7e5-110">Typ</span><span class="sxs-lookup"><span data-stu-id="4b7e5-110">Type</span></span>|<span data-ttu-id="4b7e5-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4b7e5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b7e5-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="4b7e5-112">movieRating</span></span>|[<span data-ttu-id="4b7e5-113">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="4b7e5-113">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="4b7e5-114">Bewertung für Frankreich ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="4b7e5-114">Movies rating selected for France.</span></span> <span data-ttu-id="4b7e5-115">Mögliche Werte sind: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="4b7e5-115">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="4b7e5-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="4b7e5-116">tvRating</span></span>|[<span data-ttu-id="4b7e5-117">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="4b7e5-117">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="4b7e5-118">TV-Bewertung für Frankreich ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="4b7e5-118">TV rating selected for France.</span></span> <span data-ttu-id="4b7e5-119">Mögliche Werte sind: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="4b7e5-119">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b7e5-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4b7e5-120">Relationships</span></span>
<span data-ttu-id="4b7e5-121">Keine</span><span class="sxs-lookup"><span data-stu-id="4b7e5-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b7e5-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4b7e5-122">JSON Representation</span></span>
<span data-ttu-id="4b7e5-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4b7e5-123">Here is a JSON representation of the resource.</span></span>
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




