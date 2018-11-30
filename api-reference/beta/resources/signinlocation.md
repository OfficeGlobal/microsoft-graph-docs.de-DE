---
title: Ressourcentyp signInLocation
description: Enthält den Ort, Bundesland und Land/Region aus, in dem die Anmeldung bei der.
ms.openlocfilehash: a3d4f6ca5ec18e70960f45a3da1bb06d51ee1e65
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062240"
---
# <a name="signinlocation-resource-type"></a><span data-ttu-id="c4e38-103">Ressourcentyp signInLocation</span><span class="sxs-lookup"><span data-stu-id="c4e38-103">signInLocation resource type</span></span>
<span data-ttu-id="c4e38-104">Enthält den Ort, Bundesland und Land/Region aus, in dem die Anmeldung bei der.</span><span class="sxs-lookup"><span data-stu-id="c4e38-104">Provides the city, state and country/region from where the sign-in happened.</span></span>



## <a name="properties"></a><span data-ttu-id="c4e38-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c4e38-105">Properties</span></span>
| <span data-ttu-id="c4e38-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c4e38-106">Property</span></span>     | <span data-ttu-id="c4e38-107">Typ</span><span class="sxs-lookup"><span data-stu-id="c4e38-107">Type</span></span>   |<span data-ttu-id="c4e38-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c4e38-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4e38-109">city</span><span class="sxs-lookup"><span data-stu-id="c4e38-109">city</span></span>|<span data-ttu-id="c4e38-110">String</span><span class="sxs-lookup"><span data-stu-id="c4e38-110">String</span></span>|<span data-ttu-id="c4e38-111">Enthält den Ort, von dem die Anmeldung stammt.</span><span class="sxs-lookup"><span data-stu-id="c4e38-111">Provides the city where the sign-in originated.</span></span> <span data-ttu-id="c4e38-112">Dadurch wird die anhand von Informationen aus der Aktivität Anmeldung Breitengrad/Längengrad berechnet.</span><span class="sxs-lookup"><span data-stu-id="c4e38-112">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="c4e38-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="c4e38-113">countryOrRegion</span></span>|<span data-ttu-id="c4e38-114">String</span><span class="sxs-lookup"><span data-stu-id="c4e38-114">String</span></span>|<span data-ttu-id="c4e38-115">Enthält das Land Code Info (2 Buchstaben Code), von dem die Anmeldung stammt.</span><span class="sxs-lookup"><span data-stu-id="c4e38-115">Provides the country code info (2 letter code) where the sign-in originated.</span></span>  <span data-ttu-id="c4e38-116">Dadurch wird die anhand von Informationen aus der Aktivität Anmeldung Breitengrad/Längengrad berechnet.</span><span class="sxs-lookup"><span data-stu-id="c4e38-116">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="c4e38-117">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="c4e38-117">geoCoordinates</span></span>|[<span data-ttu-id="c4e38-118">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="c4e38-118">geoCoordinates</span></span>](geocoordinates.md)|<span data-ttu-id="c4e38-119">Enthält die Breitengrad, Längengrad und Höhe, von dem die Anmeldung stammt.</span><span class="sxs-lookup"><span data-stu-id="c4e38-119">Provides the latitude, longitude and altitude where the sign-in originated.</span></span>|
|<span data-ttu-id="c4e38-120">state</span><span class="sxs-lookup"><span data-stu-id="c4e38-120">state</span></span>|<span data-ttu-id="c4e38-121">String</span><span class="sxs-lookup"><span data-stu-id="c4e38-121">String</span></span>|<span data-ttu-id="c4e38-122">Enthält den Status, in dem die Anmeldung ausgelöst hat.</span><span class="sxs-lookup"><span data-stu-id="c4e38-122">Provides the State where the sign-in originated.</span></span> <span data-ttu-id="c4e38-123">Dadurch wird die anhand von Informationen aus der Aktivität Anmeldung Breitengrad/Längengrad berechnet.</span><span class="sxs-lookup"><span data-stu-id="c4e38-123">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c4e38-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c4e38-124">JSON representation</span></span>

<span data-ttu-id="c4e38-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c4e38-125">Here is a JSON representation of the resource.</span></span>

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