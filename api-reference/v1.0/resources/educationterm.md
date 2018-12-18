---
title: educationTerm-Ressourcentyp
description: Ein Zeitraum. Er stellt einen festgelegten Teil des akademischen Jahres dar. Er wird in educationClass verwendet.
author: mmast-msft
ms.openlocfilehash: 319eedbaebde4f1e76c2f1b3e124c0dad2642538
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353088"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="5845c-105">educationTerm-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5845c-105">educationTerm resource type</span></span>

<span data-ttu-id="5845c-106">Ein Zeitraum.</span><span class="sxs-lookup"><span data-stu-id="5845c-106">A term.</span></span> <span data-ttu-id="5845c-107">Er stellt einen festgelegten Teil des akademischen Jahres dar.</span><span class="sxs-lookup"><span data-stu-id="5845c-107">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="5845c-108">Er wird in [educationClass](educationclass.md) verwendet.</span><span class="sxs-lookup"><span data-stu-id="5845c-108">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5845c-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5845c-109">Properties</span></span>
| <span data-ttu-id="5845c-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5845c-110">Property</span></span>     | <span data-ttu-id="5845c-111">Typ</span><span class="sxs-lookup"><span data-stu-id="5845c-111">Type</span></span>   |<span data-ttu-id="5845c-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5845c-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5845c-113">displayName</span><span class="sxs-lookup"><span data-stu-id="5845c-113">displayName</span></span>| <span data-ttu-id="5845c-114">String</span><span class="sxs-lookup"><span data-stu-id="5845c-114">String</span></span>| <span data-ttu-id="5845c-115">Der Anzeigename des Zeitraums</span><span class="sxs-lookup"><span data-stu-id="5845c-115">Display name of the term.</span></span>| 
|<span data-ttu-id="5845c-116">externalId</span><span class="sxs-lookup"><span data-stu-id="5845c-116">externalId</span></span>|<span data-ttu-id="5845c-117">String</span><span class="sxs-lookup"><span data-stu-id="5845c-117">String</span></span>| <span data-ttu-id="5845c-118">Die ID des Zeitraums im Synchronisierungssystem</span><span class="sxs-lookup"><span data-stu-id="5845c-118">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="5845c-119">startDate</span><span class="sxs-lookup"><span data-stu-id="5845c-119">startDate</span></span>|<span data-ttu-id="5845c-120">Date</span><span class="sxs-lookup"><span data-stu-id="5845c-120">Date</span></span>|<span data-ttu-id="5845c-121">Anfang des Zeitraums</span><span class="sxs-lookup"><span data-stu-id="5845c-121">Start of the term.</span></span>|
|<span data-ttu-id="5845c-122">endDate</span><span class="sxs-lookup"><span data-stu-id="5845c-122">endDate</span></span>|<span data-ttu-id="5845c-123">Date</span><span class="sxs-lookup"><span data-stu-id="5845c-123">Date</span></span>|<span data-ttu-id="5845c-124">Ende des Zeitraums</span><span class="sxs-lookup"><span data-stu-id="5845c-124">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5845c-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5845c-125">JSON representation</span></span>

<span data-ttu-id="5845c-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5845c-126">The following is a JSON representation of the resource.</span></span>

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