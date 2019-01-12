---
title: mediaContentRatingIreland-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9516c98350c239393e735008e91d966f8c6ae7a2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957998"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="1838a-103">mediaContentRatingIreland-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1838a-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="1838a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1838a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1838a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1838a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1838a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1838a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1838a-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="1838a-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="1838a-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1838a-108">Properties</span></span>
|<span data-ttu-id="1838a-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1838a-109">Property</span></span>|<span data-ttu-id="1838a-110">Typ</span><span class="sxs-lookup"><span data-stu-id="1838a-110">Type</span></span>|<span data-ttu-id="1838a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1838a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1838a-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="1838a-112">movieRating</span></span>|[<span data-ttu-id="1838a-113">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="1838a-113">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="1838a-114">Bewertung für Irland ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="1838a-114">Movies rating selected for Ireland.</span></span> <span data-ttu-id="1838a-115">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16` und `adults`.</span><span class="sxs-lookup"><span data-stu-id="1838a-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="1838a-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="1838a-116">tvRating</span></span>|[<span data-ttu-id="1838a-117">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="1838a-117">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="1838a-118">TV-Bewertung für Irland ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="1838a-118">TV rating selected for Ireland.</span></span> <span data-ttu-id="1838a-119">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="1838a-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1838a-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1838a-120">Relationships</span></span>
<span data-ttu-id="1838a-121">Keine</span><span class="sxs-lookup"><span data-stu-id="1838a-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1838a-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1838a-122">JSON Representation</span></span>
<span data-ttu-id="1838a-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1838a-123">Here is a JSON representation of the resource.</span></span>
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





