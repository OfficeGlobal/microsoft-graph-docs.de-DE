---
title: outlookGeoCoordinates-Ressourcentyp
description: Die geografischen Koordinaten, die Erhebung und deren Genauigkeitsgrad für einen physischen Ort.
ms.openlocfilehash: 9de60c218f6fc54ed2be12b2987126195e5eb140
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060309"
---
# <a name="outlookgeocoordinates-resource-type"></a><span data-ttu-id="8bc00-103">outlookGeoCoordinates-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8bc00-103">outlookGeoCoordinates resource type</span></span>

> <span data-ttu-id="8bc00-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8bc00-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8bc00-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8bc00-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8bc00-106">Die geografischen Koordinaten, die Erhebung und deren Genauigkeitsgrad für einen physischen Ort.</span><span class="sxs-lookup"><span data-stu-id="8bc00-106">The geographic coordinates, elevation, and their degree of accuracy for a physical location.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8bc00-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8bc00-107">JSON representation</span></span>

<span data-ttu-id="8bc00-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8bc00-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="8bc00-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8bc00-109">Properties</span></span>
| <span data-ttu-id="8bc00-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8bc00-110">Property</span></span>     | <span data-ttu-id="8bc00-111">Typ</span><span class="sxs-lookup"><span data-stu-id="8bc00-111">Type</span></span>   |<span data-ttu-id="8bc00-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8bc00-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8bc00-113">accuracy</span><span class="sxs-lookup"><span data-stu-id="8bc00-113">accuracy</span></span>|<span data-ttu-id="8bc00-114">double</span><span class="sxs-lookup"><span data-stu-id="8bc00-114">double</span></span>|<span data-ttu-id="8bc00-115">Die Genauigkeit des Breiten- und Längengrads.</span><span class="sxs-lookup"><span data-stu-id="8bc00-115">The accuracy of the latitude and longitude.</span></span> <span data-ttu-id="8bc00-116">Die Genauigkeit kann beispielsweise in Metern gemessen werden, der Breiten- und Längengrad sind beispielsweise auf 50 Meter genau.</span><span class="sxs-lookup"><span data-stu-id="8bc00-116">As an example, the accuracy can be measured in meters, such as the latitude and longitude are accurate to within 50 meters.</span></span>|
|<span data-ttu-id="8bc00-117">altitude</span><span class="sxs-lookup"><span data-stu-id="8bc00-117">altitude</span></span>|<span data-ttu-id="8bc00-118">double</span><span class="sxs-lookup"><span data-stu-id="8bc00-118">double</span></span>|<span data-ttu-id="8bc00-119">Die Höhe des Orts.</span><span class="sxs-lookup"><span data-stu-id="8bc00-119">The altitude of the location.</span></span>|
|<span data-ttu-id="8bc00-120">altitudeAccuracy</span><span class="sxs-lookup"><span data-stu-id="8bc00-120">altitudeAccuracy</span></span>|<span data-ttu-id="8bc00-121">double</span><span class="sxs-lookup"><span data-stu-id="8bc00-121">double</span></span>|<span data-ttu-id="8bc00-122">Die Genauigkeit der Höhe.</span><span class="sxs-lookup"><span data-stu-id="8bc00-122">The accuracy of the altitude.</span></span>|
|<span data-ttu-id="8bc00-123">latitude</span><span class="sxs-lookup"><span data-stu-id="8bc00-123">latitude</span></span>|<span data-ttu-id="8bc00-124">double</span><span class="sxs-lookup"><span data-stu-id="8bc00-124">double</span></span>|<span data-ttu-id="8bc00-125">Der Breitengrad des Orts.</span><span class="sxs-lookup"><span data-stu-id="8bc00-125">The latitude of the location.</span></span>|
|<span data-ttu-id="8bc00-126">longitude</span><span class="sxs-lookup"><span data-stu-id="8bc00-126">longitude</span></span>|<span data-ttu-id="8bc00-127">double</span><span class="sxs-lookup"><span data-stu-id="8bc00-127">double</span></span>|<span data-ttu-id="8bc00-128">Der Längengrad des Orts.</span><span class="sxs-lookup"><span data-stu-id="8bc00-128">The longitude of the location.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->