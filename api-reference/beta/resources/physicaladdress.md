---
title: physicalAddress-Ressourcentyp
description: Stellt die Adresse einer Ressource, z. B. eines Kontakts oder Ereignisses, dar.
localization_priority: Normal
ms.openlocfilehash: 3a656046cc23394fc8cff9100eb5ad2289050b25
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823583"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="dfc3f-103">physicalAddress-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="dfc3f-103">physicalAddress resource type</span></span>

<span data-ttu-id="dfc3f-104">Stellt die Adresse einer Ressource, z. B. eines Kontakts oder Ereignisses, dar.</span><span class="sxs-lookup"><span data-stu-id="dfc3f-104">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="dfc3f-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dfc3f-105">Properties</span></span>
| <span data-ttu-id="dfc3f-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dfc3f-106">Property</span></span>     | <span data-ttu-id="dfc3f-107">Typ</span><span class="sxs-lookup"><span data-stu-id="dfc3f-107">Type</span></span>   |<span data-ttu-id="dfc3f-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dfc3f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dfc3f-109">type</span><span class="sxs-lookup"><span data-stu-id="dfc3f-109">type</span></span>|<span data-ttu-id="dfc3f-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dfc3f-110">String</span></span>|<span data-ttu-id="dfc3f-111">Die Art der Adresse.</span><span class="sxs-lookup"><span data-stu-id="dfc3f-111">The type of address.</span></span> <span data-ttu-id="dfc3f-112">Mögliche Werte: sind `unknown`, `home`, `business` und `other`.</span><span class="sxs-lookup"><span data-stu-id="dfc3f-112">Possible values are: `unknown`, `home`, `business`, `other`.</span></span>|
|<span data-ttu-id="dfc3f-113">postOfficeBox</span><span class="sxs-lookup"><span data-stu-id="dfc3f-113">postOfficeBox</span></span>|<span data-ttu-id="dfc3f-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dfc3f-114">String</span></span>|<span data-ttu-id="dfc3f-115">Die Postfachnummer.</span><span class="sxs-lookup"><span data-stu-id="dfc3f-115">The post office box number.</span></span>|
|<span data-ttu-id="dfc3f-116">Ort</span><span class="sxs-lookup"><span data-stu-id="dfc3f-116">city</span></span>|<span data-ttu-id="dfc3f-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dfc3f-117">String</span></span>|<span data-ttu-id="dfc3f-118">Der Ort.</span><span class="sxs-lookup"><span data-stu-id="dfc3f-118">The city.</span></span>|
|<span data-ttu-id="dfc3f-119">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="dfc3f-119">countryOrRegion</span></span>|<span data-ttu-id="dfc3f-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dfc3f-120">String</span></span>|<span data-ttu-id="dfc3f-p102">Land oder Region Ein frei formatierbarer Zeichenfolgenwert, z. B. Vereinigte Staaten.</span><span class="sxs-lookup"><span data-stu-id="dfc3f-p102">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="dfc3f-123">postalCode</span><span class="sxs-lookup"><span data-stu-id="dfc3f-123">postalCode</span></span>|<span data-ttu-id="dfc3f-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dfc3f-124">String</span></span>|<span data-ttu-id="dfc3f-125">Die Postleitzahl.</span><span class="sxs-lookup"><span data-stu-id="dfc3f-125">The postal code.</span></span>|
|<span data-ttu-id="dfc3f-126">state</span><span class="sxs-lookup"><span data-stu-id="dfc3f-126">state</span></span>|<span data-ttu-id="dfc3f-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dfc3f-127">String</span></span>|<span data-ttu-id="dfc3f-128">Das Land.</span><span class="sxs-lookup"><span data-stu-id="dfc3f-128">The state.</span></span>|
|<span data-ttu-id="dfc3f-129">street</span><span class="sxs-lookup"><span data-stu-id="dfc3f-129">street</span></span>|<span data-ttu-id="dfc3f-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dfc3f-130">String</span></span>|<span data-ttu-id="dfc3f-131">Die Straße.</span><span class="sxs-lookup"><span data-stu-id="dfc3f-131">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dfc3f-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="dfc3f-132">JSON representation</span></span>

<span data-ttu-id="dfc3f-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="dfc3f-133">Here is a JSON representation of the resource</span></span>

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
