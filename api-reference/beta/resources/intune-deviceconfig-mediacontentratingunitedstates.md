---
title: mediaContentRatingUnitedStates-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cebfd525eb77c3e6e939605b80693e733f594e7d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912610"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="e48ba-103">mediaContentRatingUnitedStates-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e48ba-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="e48ba-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e48ba-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e48ba-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e48ba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e48ba-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e48ba-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e48ba-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e48ba-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="e48ba-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e48ba-108">Properties</span></span>
|<span data-ttu-id="e48ba-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e48ba-109">Property</span></span>|<span data-ttu-id="e48ba-110">Typ</span><span class="sxs-lookup"><span data-stu-id="e48ba-110">Type</span></span>|<span data-ttu-id="e48ba-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e48ba-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e48ba-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="e48ba-112">movieRating</span></span>|[<span data-ttu-id="e48ba-113">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="e48ba-113">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="e48ba-114">Bewertung für USA ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="e48ba-114">Movies rating selected for United States.</span></span> <span data-ttu-id="e48ba-115">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted` und `adults`.</span><span class="sxs-lookup"><span data-stu-id="e48ba-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="e48ba-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="e48ba-116">tvRating</span></span>|[<span data-ttu-id="e48ba-117">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="e48ba-117">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="e48ba-118">TV-Bewertung für die USA ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="e48ba-118">TV rating selected for United States.</span></span> <span data-ttu-id="e48ba-119">Mögliche Werte: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="e48ba-119">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e48ba-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e48ba-120">Relationships</span></span>
<span data-ttu-id="e48ba-121">Keine</span><span class="sxs-lookup"><span data-stu-id="e48ba-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e48ba-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e48ba-122">JSON Representation</span></span>
<span data-ttu-id="e48ba-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e48ba-123">Here is a JSON representation of the resource.</span></span>
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





