---
title: educationTerm-Ressourcentyp
description: Ein Zeitraum. Er stellt einen festgelegten Teil des akademischen Jahres dar. Er wird in educationClass verwendet.
author: mmast-msft
ms.openlocfilehash: 31925f336dbb0ce0f83ffd6b36b38e7a0916cdb5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303451"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="3bb57-105">educationTerm-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3bb57-105">educationTerm resource type</span></span>

> <span data-ttu-id="3bb57-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3bb57-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3bb57-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3bb57-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3bb57-108">Ein Zeitraum.</span><span class="sxs-lookup"><span data-stu-id="3bb57-108">A term.</span></span> <span data-ttu-id="3bb57-109">Er stellt einen festgelegten Teil des akademischen Jahres dar.</span><span class="sxs-lookup"><span data-stu-id="3bb57-109">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="3bb57-110">Er wird in [educationClass](educationclass.md) verwendet.</span><span class="sxs-lookup"><span data-stu-id="3bb57-110">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3bb57-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3bb57-111">Properties</span></span>
| <span data-ttu-id="3bb57-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3bb57-112">Property</span></span>     | <span data-ttu-id="3bb57-113">Typ</span><span class="sxs-lookup"><span data-stu-id="3bb57-113">Type</span></span>   |<span data-ttu-id="3bb57-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3bb57-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3bb57-115">displayName</span><span class="sxs-lookup"><span data-stu-id="3bb57-115">displayName</span></span>| <span data-ttu-id="3bb57-116">String</span><span class="sxs-lookup"><span data-stu-id="3bb57-116">String</span></span>| <span data-ttu-id="3bb57-117">Der Anzeigename des Zeitraums</span><span class="sxs-lookup"><span data-stu-id="3bb57-117">Display name of the term.</span></span>| 
|<span data-ttu-id="3bb57-118">externalId</span><span class="sxs-lookup"><span data-stu-id="3bb57-118">externalId</span></span>|<span data-ttu-id="3bb57-119">String</span><span class="sxs-lookup"><span data-stu-id="3bb57-119">String</span></span>| <span data-ttu-id="3bb57-120">Die ID des Zeitraums im Synchronisierungssystem</span><span class="sxs-lookup"><span data-stu-id="3bb57-120">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="3bb57-121">startDate</span><span class="sxs-lookup"><span data-stu-id="3bb57-121">startDate</span></span>|<span data-ttu-id="3bb57-122">Date</span><span class="sxs-lookup"><span data-stu-id="3bb57-122">Date</span></span>|<span data-ttu-id="3bb57-123">Anfang des Zeitraums</span><span class="sxs-lookup"><span data-stu-id="3bb57-123">Start of the term.</span></span>|
|<span data-ttu-id="3bb57-124">endDate</span><span class="sxs-lookup"><span data-stu-id="3bb57-124">endDate</span></span>|<span data-ttu-id="3bb57-125">Date</span><span class="sxs-lookup"><span data-stu-id="3bb57-125">Date</span></span>|<span data-ttu-id="3bb57-126">Ende des Zeitraums</span><span class="sxs-lookup"><span data-stu-id="3bb57-126">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3bb57-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3bb57-127">JSON representation</span></span>

<span data-ttu-id="3bb57-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3bb57-128">The following is a JSON representation of the resource.</span></span>

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