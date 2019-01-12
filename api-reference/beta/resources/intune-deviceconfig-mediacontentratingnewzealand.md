---
title: mediaContentRatingNewZealand-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a1866a6bf0c8d1849eb2fbf478b4f5d14fa3e5c0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916936"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="2a163-103">mediaContentRatingNewZealand-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2a163-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="2a163-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2a163-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2a163-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2a163-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2a163-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2a163-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a163-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="2a163-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="2a163-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2a163-108">Properties</span></span>
|<span data-ttu-id="2a163-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2a163-109">Property</span></span>|<span data-ttu-id="2a163-110">Typ</span><span class="sxs-lookup"><span data-stu-id="2a163-110">Type</span></span>|<span data-ttu-id="2a163-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2a163-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a163-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="2a163-112">movieRating</span></span>|[<span data-ttu-id="2a163-113">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="2a163-113">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="2a163-114">Bewertung für Neuseeland ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="2a163-114">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="2a163-115">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="2a163-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="2a163-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="2a163-116">tvRating</span></span>|[<span data-ttu-id="2a163-117">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="2a163-117">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="2a163-118">TV-Bewertung für Neuseeland ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="2a163-118">TV rating selected for New Zealand.</span></span> <span data-ttu-id="2a163-119">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance` und `adults`.</span><span class="sxs-lookup"><span data-stu-id="2a163-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a163-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2a163-120">Relationships</span></span>
<span data-ttu-id="2a163-121">Keine</span><span class="sxs-lookup"><span data-stu-id="2a163-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2a163-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2a163-122">JSON Representation</span></span>
<span data-ttu-id="2a163-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2a163-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```





