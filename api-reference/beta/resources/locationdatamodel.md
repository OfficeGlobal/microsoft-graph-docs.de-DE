---
title: locationDataModel-Ressourcentyp
description: Stellt locationDataModel-Informationen eines Ereignisses dar.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 2b1fd0c25cdd41e6a8d9c87f8a1c0c80d70b78e5
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057379"
---
# <a name="locationdatamodel-resource-type"></a><span data-ttu-id="588bd-103">locationDataModel-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="588bd-103">locationDataModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="588bd-104">Stellt Standortinformationen für eine Besprechung dar.</span><span class="sxs-lookup"><span data-stu-id="588bd-104">Represents location information for a meeting.</span></span>


## <a name="properties"></a><span data-ttu-id="588bd-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="588bd-105">Properties</span></span>
| <span data-ttu-id="588bd-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="588bd-106">Property</span></span>  | <span data-ttu-id="588bd-107">Typ</span><span class="sxs-lookup"><span data-stu-id="588bd-107">Type</span></span>   | <span data-ttu-id="588bd-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="588bd-108">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="588bd-109">address</span><span class="sxs-lookup"><span data-stu-id="588bd-109">address</span></span> | [<span data-ttu-id="588bd-110">postalAddress</span><span class="sxs-lookup"><span data-stu-id="588bd-110">postalAddress</span></span>](postaladdress.md) |<span data-ttu-id="588bd-111">Die Adresse des Orts.</span><span class="sxs-lookup"><span data-stu-id="588bd-111">The street address of the location.</span></span> |
| <span data-ttu-id="588bd-112">Koordinaten</span><span class="sxs-lookup"><span data-stu-id="588bd-112">coordinates</span></span> | [<span data-ttu-id="588bd-113">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="588bd-113">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="588bd-114">Die geografischen Koordinaten und die Erhebung des Orts.</span><span class="sxs-lookup"><span data-stu-id="588bd-114">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="588bd-115">displayName</span><span class="sxs-lookup"><span data-stu-id="588bd-115">displayName</span></span>  | <span data-ttu-id="588bd-116">String</span><span class="sxs-lookup"><span data-stu-id="588bd-116">String</span></span> | <span data-ttu-id="588bd-117">Der Name, der mit dem Ort verknüpft ist</span><span class="sxs-lookup"><span data-stu-id="588bd-117">The name associated with the location.</span></span>                       |
| <span data-ttu-id="588bd-118">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="588bd-118">locationEmailAddress</span></span> | <span data-ttu-id="588bd-119">String</span><span class="sxs-lookup"><span data-stu-id="588bd-119">String</span></span> | <span data-ttu-id="588bd-120">Optionale E-Mail-Adresse des Orts.</span><span class="sxs-lookup"><span data-stu-id="588bd-120">Optional email address of the location.</span></span> |
| <span data-ttu-id="588bd-121">locationUri</span><span class="sxs-lookup"><span data-stu-id="588bd-121">locationUri</span></span> | <span data-ttu-id="588bd-122">String</span><span class="sxs-lookup"><span data-stu-id="588bd-122">String</span></span> | <span data-ttu-id="588bd-123">Optionaler URI, der den Ort darstellt.</span><span class="sxs-lookup"><span data-stu-id="588bd-123">Optional URI representing the location.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="588bd-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="588bd-124">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.locationDataModel"
}-->
```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "coordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "displayName": "string",
  "locationEmailAddress": "string",
  "locationUri": "string"
}

```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "locationDataModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/locationdatamodel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
