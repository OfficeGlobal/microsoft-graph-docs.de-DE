---
title: mediaContentRatingUnitedStates-Ressourcentyp
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 60f673e31014eb4da027a58ea29099d9d8aa18e3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425834"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="8fc2f-103">mediaContentRatingUnitedStates-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8fc2f-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="8fc2f-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="8fc2f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8fc2f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8fc2f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8fc2f-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8fc2f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fc2f-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="8fc2f-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8fc2f-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8fc2f-108">Properties</span></span>
|<span data-ttu-id="8fc2f-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8fc2f-109">Property</span></span>|<span data-ttu-id="8fc2f-110">Typ</span><span class="sxs-lookup"><span data-stu-id="8fc2f-110">Type</span></span>|<span data-ttu-id="8fc2f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8fc2f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fc2f-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="8fc2f-112">movieRating</span></span>|[<span data-ttu-id="8fc2f-113">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="8fc2f-113">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="8fc2f-114">Bewertung für USA ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="8fc2f-114">Movies rating selected for United States.</span></span> <span data-ttu-id="8fc2f-115">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted` und `adults`.</span><span class="sxs-lookup"><span data-stu-id="8fc2f-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="8fc2f-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="8fc2f-116">tvRating</span></span>|[<span data-ttu-id="8fc2f-117">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="8fc2f-117">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="8fc2f-118">TV-Bewertung für die USA ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="8fc2f-118">TV rating selected for United States.</span></span> <span data-ttu-id="8fc2f-119">Mögliche Werte: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="8fc2f-119">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8fc2f-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8fc2f-120">Relationships</span></span>
<span data-ttu-id="8fc2f-121">Keine</span><span class="sxs-lookup"><span data-stu-id="8fc2f-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8fc2f-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8fc2f-122">JSON Representation</span></span>
<span data-ttu-id="8fc2f-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8fc2f-123">Here is a JSON representation of the resource.</span></span>
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




