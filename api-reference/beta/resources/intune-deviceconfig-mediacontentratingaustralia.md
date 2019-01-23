---
title: mediaContentRatingAustralia-Ressourcentyp
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 259860387e005f7fe5bfd2d402be5c03ef21149f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396637"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="e1f1f-103">mediaContentRatingAustralia-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e1f1f-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="e1f1f-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="e1f1f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e1f1f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e1f1f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e1f1f-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e1f1f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1f1f-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e1f1f-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e1f1f-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e1f1f-108">Properties</span></span>
|<span data-ttu-id="e1f1f-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e1f1f-109">Property</span></span>|<span data-ttu-id="e1f1f-110">Typ</span><span class="sxs-lookup"><span data-stu-id="e1f1f-110">Type</span></span>|<span data-ttu-id="e1f1f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e1f1f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1f1f-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="e1f1f-112">movieRating</span></span>|[<span data-ttu-id="e1f1f-113">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="e1f1f-113">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="e1f1f-114">Bewertung für Australien ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="e1f1f-114">Movies rating selected for Australia.</span></span> <span data-ttu-id="e1f1f-115">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="e1f1f-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="e1f1f-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="e1f1f-116">tvRating</span></span>|[<span data-ttu-id="e1f1f-117">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="e1f1f-117">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="e1f1f-118">TV-Bewertung für Australien ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="e1f1f-118">TV rating selected for Australia.</span></span> <span data-ttu-id="e1f1f-119">Mögliche Werte: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="e1f1f-119">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1f1f-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e1f1f-120">Relationships</span></span>
<span data-ttu-id="e1f1f-121">Keine</span><span class="sxs-lookup"><span data-stu-id="e1f1f-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1f1f-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e1f1f-122">JSON Representation</span></span>
<span data-ttu-id="e1f1f-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e1f1f-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```




