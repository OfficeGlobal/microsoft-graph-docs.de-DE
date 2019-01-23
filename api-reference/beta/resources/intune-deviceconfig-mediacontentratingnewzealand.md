---
title: mediaContentRatingNewZealand-Ressourcentyp
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: adfc34cf65104f0bf370a4e1ba22cfcb78bf250b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403448"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="19d45-103">mediaContentRatingNewZealand-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="19d45-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="19d45-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="19d45-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="19d45-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19d45-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="19d45-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="19d45-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19d45-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="19d45-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="19d45-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="19d45-108">Properties</span></span>
|<span data-ttu-id="19d45-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="19d45-109">Property</span></span>|<span data-ttu-id="19d45-110">Typ</span><span class="sxs-lookup"><span data-stu-id="19d45-110">Type</span></span>|<span data-ttu-id="19d45-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="19d45-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19d45-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="19d45-112">movieRating</span></span>|[<span data-ttu-id="19d45-113">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="19d45-113">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="19d45-114">Bewertung für Neuseeland ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="19d45-114">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="19d45-115">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="19d45-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="19d45-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="19d45-116">tvRating</span></span>|[<span data-ttu-id="19d45-117">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="19d45-117">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="19d45-118">TV-Bewertung für Neuseeland ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="19d45-118">TV rating selected for New Zealand.</span></span> <span data-ttu-id="19d45-119">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance` und `adults`.</span><span class="sxs-lookup"><span data-stu-id="19d45-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="19d45-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="19d45-120">Relationships</span></span>
<span data-ttu-id="19d45-121">Keine</span><span class="sxs-lookup"><span data-stu-id="19d45-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="19d45-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="19d45-122">JSON Representation</span></span>
<span data-ttu-id="19d45-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="19d45-123">Here is a JSON representation of the resource.</span></span>
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




