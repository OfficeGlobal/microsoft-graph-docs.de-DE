---
title: mediaContentRatingNewZealand-Ressourcentyp
description: Noch nicht dokumentiert
ms.openlocfilehash: e7650d7155c06ff30b541d873830865bed1d92ee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065440"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="7e431-103">mediaContentRatingNewZealand-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7e431-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="7e431-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7e431-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7e431-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7e431-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7e431-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7e431-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7e431-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="7e431-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="7e431-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7e431-108">Properties</span></span>
|<span data-ttu-id="7e431-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7e431-109">Property</span></span>|<span data-ttu-id="7e431-110">Typ</span><span class="sxs-lookup"><span data-stu-id="7e431-110">Type</span></span>|<span data-ttu-id="7e431-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7e431-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e431-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="7e431-112">movieRating</span></span>|[<span data-ttu-id="7e431-113">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="7e431-113">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="7e431-114">Bewertung für Neuseeland ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="7e431-114">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="7e431-115">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="7e431-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="7e431-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="7e431-116">tvRating</span></span>|[<span data-ttu-id="7e431-117">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="7e431-117">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="7e431-118">TV-Bewertung für Neuseeland ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="7e431-118">TV rating selected for New Zealand.</span></span> <span data-ttu-id="7e431-119">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance` und `adults`.</span><span class="sxs-lookup"><span data-stu-id="7e431-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e431-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7e431-120">Relationships</span></span>
<span data-ttu-id="7e431-121">Keine</span><span class="sxs-lookup"><span data-stu-id="7e431-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7e431-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7e431-122">JSON Representation</span></span>
<span data-ttu-id="7e431-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7e431-123">Here is a JSON representation of the resource.</span></span>
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





