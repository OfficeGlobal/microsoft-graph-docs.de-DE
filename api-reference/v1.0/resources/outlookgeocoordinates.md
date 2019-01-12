---
title: outlookGeoCoordinates-Ressourcentyp
description: Die geografischen Koordinaten, die Erhebung und deren Genauigkeitsgrad für einen physischen Ort.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 59b5055118cd4a213d59fdcb4921544e3b84608e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976492"
---
# <a name="outlookgeocoordinates-resource-type"></a><span data-ttu-id="a4aa2-103">outlookGeoCoordinates-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a4aa2-103">outlookGeoCoordinates resource type</span></span>

<span data-ttu-id="a4aa2-104">Die geografischen Koordinaten, die Erhebung und deren Genauigkeitsgrad für einen physischen Ort.</span><span class="sxs-lookup"><span data-stu-id="a4aa2-104">The geographic coordinates, elevation, and their degree of accuracy for a physical location.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4aa2-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a4aa2-105">JSON representation</span></span>

<span data-ttu-id="a4aa2-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a4aa2-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookGeoCoordinates"
}-->

```json
{
  "accuracy": 1024.13,
  "altitude": 1024.13,
  "altitudeAccuracy": 1024.13,
  "latitude": 1024.13,
  "longitude": 1024.13
}

```
## <a name="properties"></a><span data-ttu-id="a4aa2-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a4aa2-107">Properties</span></span>
| <span data-ttu-id="a4aa2-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a4aa2-108">Property</span></span>     | <span data-ttu-id="a4aa2-109">Typ</span><span class="sxs-lookup"><span data-stu-id="a4aa2-109">Type</span></span>   |<span data-ttu-id="a4aa2-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a4aa2-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4aa2-111">accuracy</span><span class="sxs-lookup"><span data-stu-id="a4aa2-111">accuracy</span></span>|<span data-ttu-id="a4aa2-112">double</span><span class="sxs-lookup"><span data-stu-id="a4aa2-112">double</span></span>|<span data-ttu-id="a4aa2-113">Die Genauigkeit des Breiten- und Längengrads.</span><span class="sxs-lookup"><span data-stu-id="a4aa2-113">The accuracy of the latitude and longitude.</span></span> <span data-ttu-id="a4aa2-114">Die Genauigkeit kann beispielsweise in Metern gemessen werden, der Breiten- und Längengrad sind beispielsweise auf 50 Meter genau.</span><span class="sxs-lookup"><span data-stu-id="a4aa2-114">As an example, the accuracy can be measured in meters, such as the latitude and longitude are accurate to within 50 meters.</span></span>|
|<span data-ttu-id="a4aa2-115">altitude</span><span class="sxs-lookup"><span data-stu-id="a4aa2-115">altitude</span></span>|<span data-ttu-id="a4aa2-116">double</span><span class="sxs-lookup"><span data-stu-id="a4aa2-116">double</span></span>|<span data-ttu-id="a4aa2-117">Die Höhe des Orts.</span><span class="sxs-lookup"><span data-stu-id="a4aa2-117">The altitude of the location.</span></span>|
|<span data-ttu-id="a4aa2-118">altitudeAccuracy</span><span class="sxs-lookup"><span data-stu-id="a4aa2-118">altitudeAccuracy</span></span>|<span data-ttu-id="a4aa2-119">double</span><span class="sxs-lookup"><span data-stu-id="a4aa2-119">double</span></span>|<span data-ttu-id="a4aa2-120">Die Genauigkeit der Höhe.</span><span class="sxs-lookup"><span data-stu-id="a4aa2-120">The accuracy of the altitude.</span></span>|
|<span data-ttu-id="a4aa2-121">latitude</span><span class="sxs-lookup"><span data-stu-id="a4aa2-121">latitude</span></span>|<span data-ttu-id="a4aa2-122">double</span><span class="sxs-lookup"><span data-stu-id="a4aa2-122">double</span></span>|<span data-ttu-id="a4aa2-123">Der Breitengrad des Orts.</span><span class="sxs-lookup"><span data-stu-id="a4aa2-123">The latitude of the location.</span></span>|
|<span data-ttu-id="a4aa2-124">longitude</span><span class="sxs-lookup"><span data-stu-id="a4aa2-124">longitude</span></span>|<span data-ttu-id="a4aa2-125">double</span><span class="sxs-lookup"><span data-stu-id="a4aa2-125">double</span></span>|<span data-ttu-id="a4aa2-126">Der Längengrad des Orts.</span><span class="sxs-lookup"><span data-stu-id="a4aa2-126">The longitude of the location.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
