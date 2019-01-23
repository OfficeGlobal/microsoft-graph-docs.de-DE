---
title: mediaContentRatingIreland-Ressourcentyp
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b3efd96cc8ad015989365dff10b1659ef50c4fb7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422600"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="d0e3c-103">mediaContentRatingIreland-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d0e3c-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="d0e3c-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="d0e3c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d0e3c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d0e3c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d0e3c-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d0e3c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0e3c-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="d0e3c-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="d0e3c-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d0e3c-108">Properties</span></span>
|<span data-ttu-id="d0e3c-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d0e3c-109">Property</span></span>|<span data-ttu-id="d0e3c-110">Typ</span><span class="sxs-lookup"><span data-stu-id="d0e3c-110">Type</span></span>|<span data-ttu-id="d0e3c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d0e3c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0e3c-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="d0e3c-112">movieRating</span></span>|[<span data-ttu-id="d0e3c-113">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="d0e3c-113">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="d0e3c-114">Bewertung für Irland ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="d0e3c-114">Movies rating selected for Ireland.</span></span> <span data-ttu-id="d0e3c-115">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16` und `adults`.</span><span class="sxs-lookup"><span data-stu-id="d0e3c-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="d0e3c-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="d0e3c-116">tvRating</span></span>|[<span data-ttu-id="d0e3c-117">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="d0e3c-117">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="d0e3c-118">TV-Bewertung für Irland ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="d0e3c-118">TV rating selected for Ireland.</span></span> <span data-ttu-id="d0e3c-119">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="d0e3c-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0e3c-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d0e3c-120">Relationships</span></span>
<span data-ttu-id="d0e3c-121">Keine</span><span class="sxs-lookup"><span data-stu-id="d0e3c-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0e3c-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d0e3c-122">JSON Representation</span></span>
<span data-ttu-id="d0e3c-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d0e3c-123">Here is a JSON representation of the resource.</span></span>
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




