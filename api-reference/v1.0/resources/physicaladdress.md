---
title: physicalAddress-Ressourcentyp
description: Stellt die Adresse einer Ressource, z. B. eines Kontakts oder Ereignisses, dar.
ms.openlocfilehash: eb2c1ea6a73d7f6eb5d3d43b877f50dc39a2b17e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017891"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="2b558-103">physicalAddress-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2b558-103">physicalAddress resource type</span></span>

<span data-ttu-id="2b558-104">Stellt die Adresse einer Ressource, z. B. eines Kontakts oder Ereignisses, dar.</span><span class="sxs-lookup"><span data-stu-id="2b558-104">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="2b558-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2b558-105">Properties</span></span>
| <span data-ttu-id="2b558-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2b558-106">Property</span></span>     | <span data-ttu-id="2b558-107">Typ</span><span class="sxs-lookup"><span data-stu-id="2b558-107">Type</span></span>   |<span data-ttu-id="2b558-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2b558-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b558-109">city</span><span class="sxs-lookup"><span data-stu-id="2b558-109">city</span></span>|<span data-ttu-id="2b558-110">String</span><span class="sxs-lookup"><span data-stu-id="2b558-110">String</span></span>|<span data-ttu-id="2b558-111">Der Ort.</span><span class="sxs-lookup"><span data-stu-id="2b558-111">The city.</span></span>|
|<span data-ttu-id="2b558-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="2b558-112">countryOrRegion</span></span>|<span data-ttu-id="2b558-113">String</span><span class="sxs-lookup"><span data-stu-id="2b558-113">String</span></span>|<span data-ttu-id="2b558-p101">Land oder Region Ein frei formatierbarer Zeichenfolgenwert, z. B. Vereinigte Staaten.</span><span class="sxs-lookup"><span data-stu-id="2b558-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="2b558-116">postalCode</span><span class="sxs-lookup"><span data-stu-id="2b558-116">postalCode</span></span>|<span data-ttu-id="2b558-117">String</span><span class="sxs-lookup"><span data-stu-id="2b558-117">String</span></span>|<span data-ttu-id="2b558-118">Die Postleitzahl.</span><span class="sxs-lookup"><span data-stu-id="2b558-118">The postal code.</span></span>|
|<span data-ttu-id="2b558-119">state</span><span class="sxs-lookup"><span data-stu-id="2b558-119">state</span></span>|<span data-ttu-id="2b558-120">String</span><span class="sxs-lookup"><span data-stu-id="2b558-120">String</span></span>|<span data-ttu-id="2b558-121">Das Land.</span><span class="sxs-lookup"><span data-stu-id="2b558-121">The state.</span></span>|
|<span data-ttu-id="2b558-122">street</span><span class="sxs-lookup"><span data-stu-id="2b558-122">street</span></span>|<span data-ttu-id="2b558-123">String</span><span class="sxs-lookup"><span data-stu-id="2b558-123">String</span></span>|<span data-ttu-id="2b558-124">Die Straße.</span><span class="sxs-lookup"><span data-stu-id="2b558-124">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2b558-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2b558-125">JSON representation</span></span>

<span data-ttu-id="2b558-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2b558-126">Here is a JSON representation of the resource</span></span>

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
  "state": "string",
  "street": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "physicalAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
