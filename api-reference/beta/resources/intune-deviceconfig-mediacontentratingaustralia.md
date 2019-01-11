---
title: mediaContentRatingAustralia-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 916257d83e28f3877773a6fcc7d7aefadab41af8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884224"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="8e6bf-103">mediaContentRatingAustralia-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8e6bf-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="8e6bf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8e6bf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e6bf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8e6bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8e6bf-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8e6bf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e6bf-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="8e6bf-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="8e6bf-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8e6bf-108">Properties</span></span>
|<span data-ttu-id="8e6bf-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8e6bf-109">Property</span></span>|<span data-ttu-id="8e6bf-110">Typ</span><span class="sxs-lookup"><span data-stu-id="8e6bf-110">Type</span></span>|<span data-ttu-id="8e6bf-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8e6bf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e6bf-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="8e6bf-112">movieRating</span></span>|[<span data-ttu-id="8e6bf-113">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="8e6bf-113">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="8e6bf-114">Bewertung für Australien ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="8e6bf-114">Movies rating selected for Australia.</span></span> <span data-ttu-id="8e6bf-115">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="8e6bf-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="8e6bf-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="8e6bf-116">tvRating</span></span>|[<span data-ttu-id="8e6bf-117">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="8e6bf-117">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="8e6bf-118">TV-Bewertung für Australien ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="8e6bf-118">TV rating selected for Australia.</span></span> <span data-ttu-id="8e6bf-119">Mögliche Werte: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="8e6bf-119">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e6bf-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8e6bf-120">Relationships</span></span>
<span data-ttu-id="8e6bf-121">Keine</span><span class="sxs-lookup"><span data-stu-id="8e6bf-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8e6bf-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8e6bf-122">JSON Representation</span></span>
<span data-ttu-id="8e6bf-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8e6bf-123">Here is a JSON representation of the resource.</span></span>
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





