---
title: postalAddress-Ressourcentyp
description: Stellt die Adresse einer Ressource, z. B. eines Kontakts oder Ereignisses, dar.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7d168e4f53dbd182e4dbd93d0a5b6342daf3339d
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057377"
---
# <a name="postaladdress-resource-type"></a><span data-ttu-id="e25b1-103">postalAddress-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e25b1-103">postalAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e25b1-104">Stellt die Straßenadresse eines Standorts dar.</span><span class="sxs-lookup"><span data-stu-id="e25b1-104">Represents the street address of a location.</span></span>


## <a name="properties"></a><span data-ttu-id="e25b1-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e25b1-105">Properties</span></span>
| <span data-ttu-id="e25b1-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e25b1-106">Property</span></span>     | <span data-ttu-id="e25b1-107">Typ</span><span class="sxs-lookup"><span data-stu-id="e25b1-107">Type</span></span>   |<span data-ttu-id="e25b1-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e25b1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e25b1-109">city</span><span class="sxs-lookup"><span data-stu-id="e25b1-109">city</span></span>|<span data-ttu-id="e25b1-110">String</span><span class="sxs-lookup"><span data-stu-id="e25b1-110">String</span></span>|<span data-ttu-id="e25b1-111">Der Ort.</span><span class="sxs-lookup"><span data-stu-id="e25b1-111">The city.</span></span>|
|<span data-ttu-id="e25b1-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="e25b1-112">countryOrRegion</span></span>|<span data-ttu-id="e25b1-113">String</span><span class="sxs-lookup"><span data-stu-id="e25b1-113">String</span></span>|<span data-ttu-id="e25b1-p101">Land oder Region Ein frei formatierbarer Zeichenfolgenwert, z. B. Vereinigte Staaten.</span><span class="sxs-lookup"><span data-stu-id="e25b1-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="e25b1-116">isInferred</span><span class="sxs-lookup"><span data-stu-id="e25b1-116">isInferred</span></span>|<span data-ttu-id="e25b1-117">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e25b1-117">Boolean</span></span>|<span data-ttu-id="e25b1-118">Nur für internen Gebrauch.</span><span class="sxs-lookup"><span data-stu-id="e25b1-118">For internal use only.</span></span>|
|<span data-ttu-id="e25b1-119">postalCode</span><span class="sxs-lookup"><span data-stu-id="e25b1-119">postalCode</span></span>|<span data-ttu-id="e25b1-120">String</span><span class="sxs-lookup"><span data-stu-id="e25b1-120">String</span></span>|<span data-ttu-id="e25b1-121">Die Postleitzahl.</span><span class="sxs-lookup"><span data-stu-id="e25b1-121">The postal code.</span></span>|
|<span data-ttu-id="e25b1-122">state</span><span class="sxs-lookup"><span data-stu-id="e25b1-122">state</span></span>|<span data-ttu-id="e25b1-123">String</span><span class="sxs-lookup"><span data-stu-id="e25b1-123">String</span></span>|<span data-ttu-id="e25b1-124">Das Land.</span><span class="sxs-lookup"><span data-stu-id="e25b1-124">The state.</span></span>|
|<span data-ttu-id="e25b1-125">street</span><span class="sxs-lookup"><span data-stu-id="e25b1-125">street</span></span>|<span data-ttu-id="e25b1-126">String</span><span class="sxs-lookup"><span data-stu-id="e25b1-126">String</span></span>|<span data-ttu-id="e25b1-127">Die Straße.</span><span class="sxs-lookup"><span data-stu-id="e25b1-127">The street.</span></span>|
|<span data-ttu-id="e25b1-128">type</span><span class="sxs-lookup"><span data-stu-id="e25b1-128">type</span></span>|<span data-ttu-id="e25b1-129">addressType</span><span class="sxs-lookup"><span data-stu-id="e25b1-129">addressType</span></span>|<span data-ttu-id="e25b1-130">Der Adresstyp.</span><span class="sxs-lookup"><span data-stu-id="e25b1-130">The type of address.</span></span> <span data-ttu-id="e25b1-131">Die möglichen Werte sind: `unknown`, `home`, `business`, `other`.</span><span class="sxs-lookup"><span data-stu-id="e25b1-131">The possible values are: `unknown`, `home`, `business`, `other`.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e25b1-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e25b1-132">JSON representation</span></span>

<span data-ttu-id="e25b1-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e25b1-133">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.postalAddress"
}-->

```json
{
  "city": "string",
  "countryOrRegion": "string",
  "isInferred": "boolean",
  "postalCode": "string",
  "state": "string",
  "street": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "postaladdress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/postaladdress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}-->
