---
title: physicalAddress-Ressourcentyp
description: Stellt die Adresse einer Ressource, z. B. eines Kontakts oder Ereignisses, dar.
ms.openlocfilehash: 819240be3eb9a088fde43390fbb1d1d4af1fd30c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064741"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="b8d78-103">physicalAddress-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b8d78-103">physicalAddress resource type</span></span>

<span data-ttu-id="b8d78-104">Stellt die Adresse einer Ressource, z. B. eines Kontakts oder Ereignisses, dar.</span><span class="sxs-lookup"><span data-stu-id="b8d78-104">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="b8d78-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b8d78-105">Properties</span></span>
| <span data-ttu-id="b8d78-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b8d78-106">Property</span></span>     | <span data-ttu-id="b8d78-107">Typ</span><span class="sxs-lookup"><span data-stu-id="b8d78-107">Type</span></span>   |<span data-ttu-id="b8d78-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8d78-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8d78-109">Typ</span><span class="sxs-lookup"><span data-stu-id="b8d78-109">type</span></span>|<span data-ttu-id="b8d78-110">String</span><span class="sxs-lookup"><span data-stu-id="b8d78-110">String</span></span>|<span data-ttu-id="b8d78-111">Die Art der Adresse.</span><span class="sxs-lookup"><span data-stu-id="b8d78-111">The type of address.</span></span> <span data-ttu-id="b8d78-112">Mögliche Werte: sind `unknown`, `home`, `business` und `other`.</span><span class="sxs-lookup"><span data-stu-id="b8d78-112">Possible values are: `unknown`, `home`, `business`, `other`.</span></span>|
|<span data-ttu-id="b8d78-113">postOfficeBox</span><span class="sxs-lookup"><span data-stu-id="b8d78-113">postOfficeBox</span></span>|<span data-ttu-id="b8d78-114">String</span><span class="sxs-lookup"><span data-stu-id="b8d78-114">String</span></span>|<span data-ttu-id="b8d78-115">Die Postfachnummer.</span><span class="sxs-lookup"><span data-stu-id="b8d78-115">The post office box number.</span></span>|
|<span data-ttu-id="b8d78-116">Ort</span><span class="sxs-lookup"><span data-stu-id="b8d78-116">city</span></span>|<span data-ttu-id="b8d78-117">String</span><span class="sxs-lookup"><span data-stu-id="b8d78-117">String</span></span>|<span data-ttu-id="b8d78-118">Der Ort.</span><span class="sxs-lookup"><span data-stu-id="b8d78-118">The city.</span></span>|
|<span data-ttu-id="b8d78-119">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="b8d78-119">countryOrRegion</span></span>|<span data-ttu-id="b8d78-120">String</span><span class="sxs-lookup"><span data-stu-id="b8d78-120">String</span></span>|<span data-ttu-id="b8d78-p102">Land oder Region Ein frei formatierbarer Zeichenfolgenwert, z. B. Vereinigte Staaten.</span><span class="sxs-lookup"><span data-stu-id="b8d78-p102">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="b8d78-123">postalCode</span><span class="sxs-lookup"><span data-stu-id="b8d78-123">postalCode</span></span>|<span data-ttu-id="b8d78-124">String</span><span class="sxs-lookup"><span data-stu-id="b8d78-124">String</span></span>|<span data-ttu-id="b8d78-125">Die Postleitzahl.</span><span class="sxs-lookup"><span data-stu-id="b8d78-125">The postal code.</span></span>|
|<span data-ttu-id="b8d78-126">state</span><span class="sxs-lookup"><span data-stu-id="b8d78-126">state</span></span>|<span data-ttu-id="b8d78-127">String</span><span class="sxs-lookup"><span data-stu-id="b8d78-127">String</span></span>|<span data-ttu-id="b8d78-128">Das Land.</span><span class="sxs-lookup"><span data-stu-id="b8d78-128">The state.</span></span>|
|<span data-ttu-id="b8d78-129">street</span><span class="sxs-lookup"><span data-stu-id="b8d78-129">street</span></span>|<span data-ttu-id="b8d78-130">String</span><span class="sxs-lookup"><span data-stu-id="b8d78-130">String</span></span>|<span data-ttu-id="b8d78-131">Die Straße.</span><span class="sxs-lookup"><span data-stu-id="b8d78-131">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8d78-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b8d78-132">JSON representation</span></span>

<span data-ttu-id="b8d78-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b8d78-133">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.physicalAddress"
}-->

```json
{
  "type": "string",
  "postOfficeBox": "string",
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
