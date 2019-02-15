---
title: physicalAddress-Ressourcentyp
description: Stellt die Adresse einer Ressource, z. B. eines Kontakts oder Ereignisses, dar.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: eb7bf1ee21a40517704f20176f5fbcf9ea2b276a
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2019
ms.locfileid: "30056987"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="efe5c-103">physicalAddress-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="efe5c-103">physicalAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efe5c-104">Stellt die Adresse einer Ressource, z. B. eines Kontakts oder Ereignisses, dar.</span><span class="sxs-lookup"><span data-stu-id="efe5c-104">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="efe5c-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="efe5c-105">Properties</span></span>
| <span data-ttu-id="efe5c-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="efe5c-106">Property</span></span>     | <span data-ttu-id="efe5c-107">Typ</span><span class="sxs-lookup"><span data-stu-id="efe5c-107">Type</span></span>   |<span data-ttu-id="efe5c-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="efe5c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="efe5c-109">city</span><span class="sxs-lookup"><span data-stu-id="efe5c-109">city</span></span>|<span data-ttu-id="efe5c-110">String</span><span class="sxs-lookup"><span data-stu-id="efe5c-110">String</span></span>|<span data-ttu-id="efe5c-111">Der Ort.</span><span class="sxs-lookup"><span data-stu-id="efe5c-111">The city.</span></span>|
|<span data-ttu-id="efe5c-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="efe5c-112">countryOrRegion</span></span>|<span data-ttu-id="efe5c-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="efe5c-113">String</span></span>|<span data-ttu-id="efe5c-p101">Land oder Region Ein frei formatierbarer Zeichenfolgenwert, z. B. Vereinigte Staaten.</span><span class="sxs-lookup"><span data-stu-id="efe5c-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="efe5c-116">postalCode</span><span class="sxs-lookup"><span data-stu-id="efe5c-116">postalCode</span></span>|<span data-ttu-id="efe5c-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="efe5c-117">String</span></span>|<span data-ttu-id="efe5c-118">Die Postleitzahl.</span><span class="sxs-lookup"><span data-stu-id="efe5c-118">The postal code.</span></span>|
|<span data-ttu-id="efe5c-119">postOfficeBox</span><span class="sxs-lookup"><span data-stu-id="efe5c-119">postOfficeBox</span></span>|<span data-ttu-id="efe5c-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="efe5c-120">String</span></span>|<span data-ttu-id="efe5c-121">Die Postfachnummer.</span><span class="sxs-lookup"><span data-stu-id="efe5c-121">The post office box number.</span></span>|
|<span data-ttu-id="efe5c-122">state</span><span class="sxs-lookup"><span data-stu-id="efe5c-122">state</span></span>|<span data-ttu-id="efe5c-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="efe5c-123">String</span></span>|<span data-ttu-id="efe5c-124">Das Land.</span><span class="sxs-lookup"><span data-stu-id="efe5c-124">The state.</span></span>|
|<span data-ttu-id="efe5c-125">street</span><span class="sxs-lookup"><span data-stu-id="efe5c-125">street</span></span>|<span data-ttu-id="efe5c-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="efe5c-126">String</span></span>|<span data-ttu-id="efe5c-127">Die Straße.</span><span class="sxs-lookup"><span data-stu-id="efe5c-127">The street.</span></span>|
|<span data-ttu-id="efe5c-128">type</span><span class="sxs-lookup"><span data-stu-id="efe5c-128">type</span></span>|<span data-ttu-id="efe5c-129">: Physicaladdresstype</span><span class="sxs-lookup"><span data-stu-id="efe5c-129">physicalAddressType</span></span>|<span data-ttu-id="efe5c-130">Der Adresstyp.</span><span class="sxs-lookup"><span data-stu-id="efe5c-130">The type of address.</span></span> <span data-ttu-id="efe5c-131">Mögliche Werte: `unknown`, `home`, `business`, `other`.</span><span class="sxs-lookup"><span data-stu-id="efe5c-131">Possible values are: `unknown`, `home`, `business`, `other`.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="efe5c-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="efe5c-132">JSON representation</span></span>

<span data-ttu-id="efe5c-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="efe5c-133">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.physicalAddress"
}-->

```json
{
  "city": "string",
  "countryOrRegion": "string",
  "postalCode": "string",
  "postOfficeBox": "string",
  "state": "string",
  "street": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "physicalAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/physicaladdress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}-->
