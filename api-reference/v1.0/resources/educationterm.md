---
title: educationTerm-Ressourcentyp
description: Ein Zeitraum. Er stellt einen festgelegten Teil des akademischen Jahres dar. Er wird in educationClass verwendet.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 9c26565b552471fe2601d8e3cb629fd933d72937
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947582"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="44941-105">educationTerm-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="44941-105">educationTerm resource type</span></span>

<span data-ttu-id="44941-106">Ein Zeitraum.</span><span class="sxs-lookup"><span data-stu-id="44941-106">A term.</span></span> <span data-ttu-id="44941-107">Er stellt einen festgelegten Teil des akademischen Jahres dar.</span><span class="sxs-lookup"><span data-stu-id="44941-107">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="44941-108">Er wird in [educationClass](educationclass.md) verwendet.</span><span class="sxs-lookup"><span data-stu-id="44941-108">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="44941-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="44941-109">Properties</span></span>
| <span data-ttu-id="44941-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="44941-110">Property</span></span>     | <span data-ttu-id="44941-111">Typ</span><span class="sxs-lookup"><span data-stu-id="44941-111">Type</span></span>   |<span data-ttu-id="44941-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="44941-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44941-113">displayName</span><span class="sxs-lookup"><span data-stu-id="44941-113">displayName</span></span>| <span data-ttu-id="44941-114">String</span><span class="sxs-lookup"><span data-stu-id="44941-114">String</span></span>| <span data-ttu-id="44941-115">Der Anzeigename des Zeitraums</span><span class="sxs-lookup"><span data-stu-id="44941-115">Display name of the term.</span></span>| 
|<span data-ttu-id="44941-116">externalId</span><span class="sxs-lookup"><span data-stu-id="44941-116">externalId</span></span>|<span data-ttu-id="44941-117">String</span><span class="sxs-lookup"><span data-stu-id="44941-117">String</span></span>| <span data-ttu-id="44941-118">Die ID des Zeitraums im Synchronisierungssystem</span><span class="sxs-lookup"><span data-stu-id="44941-118">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="44941-119">startDate</span><span class="sxs-lookup"><span data-stu-id="44941-119">startDate</span></span>|<span data-ttu-id="44941-120">Date</span><span class="sxs-lookup"><span data-stu-id="44941-120">Date</span></span>|<span data-ttu-id="44941-121">Anfang des Zeitraums</span><span class="sxs-lookup"><span data-stu-id="44941-121">Start of the term.</span></span>|
|<span data-ttu-id="44941-122">endDate</span><span class="sxs-lookup"><span data-stu-id="44941-122">endDate</span></span>|<span data-ttu-id="44941-123">Date</span><span class="sxs-lookup"><span data-stu-id="44941-123">Date</span></span>|<span data-ttu-id="44941-124">Ende des Zeitraums</span><span class="sxs-lookup"><span data-stu-id="44941-124">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="44941-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="44941-125">JSON representation</span></span>

<span data-ttu-id="44941-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="44941-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTerm"
}-->

```json
{
  "displayName": "String",
  "externalId": "String",
  "startDate": "Date",
  "endDate": "Date"
}
```

<!-- uuid: 4e9d671f-3068-4e09-aba2-b39e81a0e452
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationTerm resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
