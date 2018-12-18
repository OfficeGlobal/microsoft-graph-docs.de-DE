---
title: mediaContentRatingGermany-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: b7e02226ccea817a609d6e7f3059bff8e6bdb9ce
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318361"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="719bd-103">mediaContentRatingGermany-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="719bd-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="719bd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="719bd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="719bd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="719bd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="719bd-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="719bd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="719bd-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="719bd-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="719bd-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="719bd-108">Properties</span></span>
|<span data-ttu-id="719bd-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="719bd-109">Property</span></span>|<span data-ttu-id="719bd-110">Typ</span><span class="sxs-lookup"><span data-stu-id="719bd-110">Type</span></span>|<span data-ttu-id="719bd-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="719bd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="719bd-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="719bd-112">movieRating</span></span>|[<span data-ttu-id="719bd-113">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="719bd-113">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="719bd-114">Bewertung für Deutschland ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="719bd-114">Movies rating selected for Germany.</span></span> <span data-ttu-id="719bd-115">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16` und `adults`.</span><span class="sxs-lookup"><span data-stu-id="719bd-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="719bd-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="719bd-116">tvRating</span></span>|[<span data-ttu-id="719bd-117">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="719bd-117">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="719bd-118">TV-Bewertung für Deutschland ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="719bd-118">TV rating selected for Germany.</span></span> <span data-ttu-id="719bd-119">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="719bd-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="719bd-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="719bd-120">Relationships</span></span>
<span data-ttu-id="719bd-121">Keine</span><span class="sxs-lookup"><span data-stu-id="719bd-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="719bd-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="719bd-122">JSON Representation</span></span>
<span data-ttu-id="719bd-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="719bd-123">Here is a JSON representation of the resource.</span></span>
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





