---
title: Ressourcentyp physicalOfficeAddress
description: Geschäftsadresse einer Ressource wie einen Kontakt oder eine Ereignis darstellt.
ms.openlocfilehash: 472e4dfd03670f5fd4ff6b5c5c53342fff5c391a
ms.sourcegitcommit: f3d479edf03935d0edbbc7668a65f7cde2a56c92
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/15/2018
ms.locfileid: "27284098"
---
# <a name="physicalofficeaddress-resource-type"></a><span data-ttu-id="445c9-103">Ressourcentyp physicalOfficeAddress</span><span class="sxs-lookup"><span data-stu-id="445c9-103">physicalOfficeAddress resource type</span></span>

<span data-ttu-id="445c9-104">Geschäftsadresse einer Ressource wie eine Organisationseinheit Kontakt darstellt.</span><span class="sxs-lookup"><span data-stu-id="445c9-104">Represents the business address of a resource such as an organizational contact.</span></span>

## <a name="properties"></a><span data-ttu-id="445c9-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="445c9-105">Properties</span></span>

| <span data-ttu-id="445c9-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="445c9-106">Property</span></span>     | <span data-ttu-id="445c9-107">Typ</span><span class="sxs-lookup"><span data-stu-id="445c9-107">Type</span></span>   |<span data-ttu-id="445c9-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="445c9-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="445c9-109">city</span><span class="sxs-lookup"><span data-stu-id="445c9-109">city</span></span>|<span data-ttu-id="445c9-110">String</span><span class="sxs-lookup"><span data-stu-id="445c9-110">String</span></span>|<span data-ttu-id="445c9-111">Der Ort.</span><span class="sxs-lookup"><span data-stu-id="445c9-111">The city.</span></span>|
|<span data-ttu-id="445c9-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="445c9-112">countryOrRegion</span></span>|<span data-ttu-id="445c9-113">String</span><span class="sxs-lookup"><span data-stu-id="445c9-113">String</span></span>|<span data-ttu-id="445c9-p101">Land oder Region Ein frei formatierbarer Zeichenfolgenwert, z. B. Vereinigte Staaten.</span><span class="sxs-lookup"><span data-stu-id="445c9-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="445c9-116">officeLocation</span><span class="sxs-lookup"><span data-stu-id="445c9-116">officeLocation</span></span>  | <span data-ttu-id="445c9-117">String</span><span class="sxs-lookup"><span data-stu-id="445c9-117">String</span></span> | <span data-ttu-id="445c9-118">Standort des Büros wie Gebäude und Office Anzahl für eine Organisationseinheit Kontakt.</span><span class="sxs-lookup"><span data-stu-id="445c9-118">Office location such as building and office number for an organizational contact.</span></span>  |
|<span data-ttu-id="445c9-119">postalCode</span><span class="sxs-lookup"><span data-stu-id="445c9-119">postalCode</span></span>|<span data-ttu-id="445c9-120">String</span><span class="sxs-lookup"><span data-stu-id="445c9-120">String</span></span>|<span data-ttu-id="445c9-121">Die Postleitzahl.</span><span class="sxs-lookup"><span data-stu-id="445c9-121">The postal code.</span></span>|
|<span data-ttu-id="445c9-122">state</span><span class="sxs-lookup"><span data-stu-id="445c9-122">state</span></span>|<span data-ttu-id="445c9-123">String</span><span class="sxs-lookup"><span data-stu-id="445c9-123">String</span></span>|<span data-ttu-id="445c9-124">Das Land.</span><span class="sxs-lookup"><span data-stu-id="445c9-124">The state.</span></span>|
|<span data-ttu-id="445c9-125">street</span><span class="sxs-lookup"><span data-stu-id="445c9-125">street</span></span>|<span data-ttu-id="445c9-126">String</span><span class="sxs-lookup"><span data-stu-id="445c9-126">String</span></span>|<span data-ttu-id="445c9-127">Die Straße.</span><span class="sxs-lookup"><span data-stu-id="445c9-127">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="445c9-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="445c9-128">JSON representation</span></span>

<span data-ttu-id="445c9-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="445c9-129">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.physicalOfficeAddress"
}-->

```json
{
  "city": "string",
  "countryOrRegion": "string",
  "officeLocation": "string",
  "postalCode": "string",
  "state": "string",
  "street": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "physicalOfficeAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
