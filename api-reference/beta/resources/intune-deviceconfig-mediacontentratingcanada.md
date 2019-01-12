---
title: mediaContentRatingCanada-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0e6b3c84801ecf1338a04e356d9141d4b45286de
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981000"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="3ea18-103">mediaContentRatingCanada-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3ea18-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="3ea18-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3ea18-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3ea18-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3ea18-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3ea18-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3ea18-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3ea18-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="3ea18-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="3ea18-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3ea18-108">Properties</span></span>
|<span data-ttu-id="3ea18-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3ea18-109">Property</span></span>|<span data-ttu-id="3ea18-110">Typ</span><span class="sxs-lookup"><span data-stu-id="3ea18-110">Type</span></span>|<span data-ttu-id="3ea18-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3ea18-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ea18-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="3ea18-112">movieRating</span></span>|[<span data-ttu-id="3ea18-113">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="3ea18-113">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="3ea18-114">Bewertung für Kanada ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="3ea18-114">Movies rating selected for Canada.</span></span> <span data-ttu-id="3ea18-115">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18` und `restricted`.</span><span class="sxs-lookup"><span data-stu-id="3ea18-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="3ea18-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="3ea18-116">tvRating</span></span>|[<span data-ttu-id="3ea18-117">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="3ea18-117">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="3ea18-118">TV-Bewertung für Kanada ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="3ea18-118">TV rating selected for Canada.</span></span> <span data-ttu-id="3ea18-119">Mögliche Werte: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="3ea18-119">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ea18-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3ea18-120">Relationships</span></span>
<span data-ttu-id="3ea18-121">Keine</span><span class="sxs-lookup"><span data-stu-id="3ea18-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3ea18-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3ea18-122">JSON Representation</span></span>
<span data-ttu-id="3ea18-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3ea18-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingCanada"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingCanada",
  "movieRating": "String",
  "tvRating": "String"
}
```





