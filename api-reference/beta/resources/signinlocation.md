---
title: Ressourcentyp signInLocation
description: Enthält den Ort, Bundesland und Land/Region aus, in dem die Anmeldung bei der.
localization_priority: Normal
ms.openlocfilehash: 49d6dfb07c635ac3754b3e873d75911a43593a73
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839137"
---
# <a name="signinlocation-resource-type"></a><span data-ttu-id="c09a5-103">Ressourcentyp signInLocation</span><span class="sxs-lookup"><span data-stu-id="c09a5-103">signInLocation resource type</span></span>
<span data-ttu-id="c09a5-104">Enthält den Ort, Bundesland und Land/Region aus, in dem die Anmeldung bei der.</span><span class="sxs-lookup"><span data-stu-id="c09a5-104">Provides the city, state and country/region from where the sign-in happened.</span></span>



## <a name="properties"></a><span data-ttu-id="c09a5-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c09a5-105">Properties</span></span>
| <span data-ttu-id="c09a5-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c09a5-106">Property</span></span>     | <span data-ttu-id="c09a5-107">Typ</span><span class="sxs-lookup"><span data-stu-id="c09a5-107">Type</span></span>   |<span data-ttu-id="c09a5-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c09a5-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c09a5-109">city</span><span class="sxs-lookup"><span data-stu-id="c09a5-109">city</span></span>|<span data-ttu-id="c09a5-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c09a5-110">String</span></span>|<span data-ttu-id="c09a5-111">Enthält den Ort, von dem die Anmeldung stammt.</span><span class="sxs-lookup"><span data-stu-id="c09a5-111">Provides the city where the sign-in originated.</span></span> <span data-ttu-id="c09a5-112">Dadurch wird die anhand von Informationen aus der Aktivität Anmeldung Breitengrad/Längengrad berechnet.</span><span class="sxs-lookup"><span data-stu-id="c09a5-112">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="c09a5-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="c09a5-113">countryOrRegion</span></span>|<span data-ttu-id="c09a5-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c09a5-114">String</span></span>|<span data-ttu-id="c09a5-115">Enthält das Land Code Info (2 Buchstaben Code), von dem die Anmeldung stammt.</span><span class="sxs-lookup"><span data-stu-id="c09a5-115">Provides the country code info (2 letter code) where the sign-in originated.</span></span>  <span data-ttu-id="c09a5-116">Dadurch wird die anhand von Informationen aus der Aktivität Anmeldung Breitengrad/Längengrad berechnet.</span><span class="sxs-lookup"><span data-stu-id="c09a5-116">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="c09a5-117">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="c09a5-117">geoCoordinates</span></span>|[<span data-ttu-id="c09a5-118">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="c09a5-118">geoCoordinates</span></span>](geocoordinates.md)|<span data-ttu-id="c09a5-119">Enthält die Breitengrad, Längengrad und Höhe, von dem die Anmeldung stammt.</span><span class="sxs-lookup"><span data-stu-id="c09a5-119">Provides the latitude, longitude and altitude where the sign-in originated.</span></span>|
|<span data-ttu-id="c09a5-120">state</span><span class="sxs-lookup"><span data-stu-id="c09a5-120">state</span></span>|<span data-ttu-id="c09a5-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c09a5-121">String</span></span>|<span data-ttu-id="c09a5-122">Enthält den Status, in dem die Anmeldung ausgelöst hat.</span><span class="sxs-lookup"><span data-stu-id="c09a5-122">Provides the State where the sign-in originated.</span></span> <span data-ttu-id="c09a5-123">Dadurch wird die anhand von Informationen aus der Aktivität Anmeldung Breitengrad/Längengrad berechnet.</span><span class="sxs-lookup"><span data-stu-id="c09a5-123">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c09a5-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c09a5-124">JSON representation</span></span>

<span data-ttu-id="c09a5-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c09a5-125">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInLocation"
}-->

```json
{
  "city": "String",
  "countryOrRegion": "String",
  "geoCoordinates": {"@odata.type": "microsoft.graph.geoCoordinates"},
  "state": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
