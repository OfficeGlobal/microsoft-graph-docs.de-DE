---
title: mediaContentRatingGermany-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 99b67a5d2f65b9ccf29ba3ce1a8c5a214f92535c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825613"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="711e5-103">mediaContentRatingGermany-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="711e5-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="711e5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="711e5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="711e5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="711e5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="711e5-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="711e5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="711e5-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="711e5-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="711e5-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="711e5-108">Properties</span></span>
|<span data-ttu-id="711e5-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="711e5-109">Property</span></span>|<span data-ttu-id="711e5-110">Typ</span><span class="sxs-lookup"><span data-stu-id="711e5-110">Type</span></span>|<span data-ttu-id="711e5-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="711e5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="711e5-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="711e5-112">movieRating</span></span>|[<span data-ttu-id="711e5-113">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="711e5-113">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="711e5-114">Bewertung für Deutschland ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="711e5-114">Movies rating selected for Germany.</span></span> <span data-ttu-id="711e5-115">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16` und `adults`.</span><span class="sxs-lookup"><span data-stu-id="711e5-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="711e5-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="711e5-116">tvRating</span></span>|[<span data-ttu-id="711e5-117">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="711e5-117">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="711e5-118">TV-Bewertung für Deutschland ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="711e5-118">TV rating selected for Germany.</span></span> <span data-ttu-id="711e5-119">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="711e5-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="711e5-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="711e5-120">Relationships</span></span>
<span data-ttu-id="711e5-121">Keine</span><span class="sxs-lookup"><span data-stu-id="711e5-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="711e5-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="711e5-122">JSON Representation</span></span>
<span data-ttu-id="711e5-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="711e5-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```





