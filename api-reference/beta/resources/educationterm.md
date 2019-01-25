---
title: educationTerm-Ressourcentyp
description: Ein Zeitraum. Er stellt einen festgelegten Teil des akademischen Jahres dar. Er wird in educationClass verwendet.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b5cfe363922fe466eef7a7333ce81249311b4063
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527563"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="ce07f-105">educationTerm-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ce07f-105">educationTerm resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce07f-106">Ein Zeitraum.</span><span class="sxs-lookup"><span data-stu-id="ce07f-106">A term.</span></span> <span data-ttu-id="ce07f-107">Er stellt einen festgelegten Teil des akademischen Jahres dar.</span><span class="sxs-lookup"><span data-stu-id="ce07f-107">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="ce07f-108">Er wird in [educationClass](educationclass.md) verwendet.</span><span class="sxs-lookup"><span data-stu-id="ce07f-108">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ce07f-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ce07f-109">Properties</span></span>
| <span data-ttu-id="ce07f-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ce07f-110">Property</span></span>     | <span data-ttu-id="ce07f-111">Typ</span><span class="sxs-lookup"><span data-stu-id="ce07f-111">Type</span></span>   |<span data-ttu-id="ce07f-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ce07f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce07f-113">displayName</span><span class="sxs-lookup"><span data-stu-id="ce07f-113">displayName</span></span>| <span data-ttu-id="ce07f-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce07f-114">String</span></span>| <span data-ttu-id="ce07f-115">Der Anzeigename des Zeitraums</span><span class="sxs-lookup"><span data-stu-id="ce07f-115">Display name of the term.</span></span>| 
|<span data-ttu-id="ce07f-116">externalId</span><span class="sxs-lookup"><span data-stu-id="ce07f-116">externalId</span></span>|<span data-ttu-id="ce07f-117">String</span><span class="sxs-lookup"><span data-stu-id="ce07f-117">String</span></span>| <span data-ttu-id="ce07f-118">Die ID des Zeitraums im Synchronisierungssystem</span><span class="sxs-lookup"><span data-stu-id="ce07f-118">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="ce07f-119">startDate</span><span class="sxs-lookup"><span data-stu-id="ce07f-119">startDate</span></span>|<span data-ttu-id="ce07f-120">Datum</span><span class="sxs-lookup"><span data-stu-id="ce07f-120">Date</span></span>|<span data-ttu-id="ce07f-121">Anfang des Zeitraums</span><span class="sxs-lookup"><span data-stu-id="ce07f-121">Start of the term.</span></span>|
|<span data-ttu-id="ce07f-122">endDate</span><span class="sxs-lookup"><span data-stu-id="ce07f-122">endDate</span></span>|<span data-ttu-id="ce07f-123">Date</span><span class="sxs-lookup"><span data-stu-id="ce07f-123">Date</span></span>|<span data-ttu-id="ce07f-124">Ende des Zeitraums</span><span class="sxs-lookup"><span data-stu-id="ce07f-124">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ce07f-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ce07f-125">JSON representation</span></span>

<span data-ttu-id="ce07f-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ce07f-126">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "educationTerm resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationterm.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
