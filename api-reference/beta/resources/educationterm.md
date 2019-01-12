---
title: educationTerm-Ressourcentyp
description: Ein Zeitraum. Er stellt einen festgelegten Teil des akademischen Jahres dar. Er wird in educationClass verwendet.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bc068df7a31c1b3903e8735ba1255cc3a6f0ae73
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962758"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="cfb45-105">educationTerm-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="cfb45-105">educationTerm resource type</span></span>

> <span data-ttu-id="cfb45-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cfb45-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cfb45-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cfb45-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cfb45-108">Ein Zeitraum.</span><span class="sxs-lookup"><span data-stu-id="cfb45-108">A term.</span></span> <span data-ttu-id="cfb45-109">Er stellt einen festgelegten Teil des akademischen Jahres dar.</span><span class="sxs-lookup"><span data-stu-id="cfb45-109">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="cfb45-110">Er wird in [educationClass](educationclass.md) verwendet.</span><span class="sxs-lookup"><span data-stu-id="cfb45-110">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="cfb45-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cfb45-111">Properties</span></span>
| <span data-ttu-id="cfb45-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cfb45-112">Property</span></span>     | <span data-ttu-id="cfb45-113">Typ</span><span class="sxs-lookup"><span data-stu-id="cfb45-113">Type</span></span>   |<span data-ttu-id="cfb45-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cfb45-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cfb45-115">displayName</span><span class="sxs-lookup"><span data-stu-id="cfb45-115">displayName</span></span>| <span data-ttu-id="cfb45-116">String</span><span class="sxs-lookup"><span data-stu-id="cfb45-116">String</span></span>| <span data-ttu-id="cfb45-117">Der Anzeigename des Zeitraums</span><span class="sxs-lookup"><span data-stu-id="cfb45-117">Display name of the term.</span></span>| 
|<span data-ttu-id="cfb45-118">externalId</span><span class="sxs-lookup"><span data-stu-id="cfb45-118">externalId</span></span>|<span data-ttu-id="cfb45-119">String</span><span class="sxs-lookup"><span data-stu-id="cfb45-119">String</span></span>| <span data-ttu-id="cfb45-120">Die ID des Zeitraums im Synchronisierungssystem</span><span class="sxs-lookup"><span data-stu-id="cfb45-120">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="cfb45-121">startDate</span><span class="sxs-lookup"><span data-stu-id="cfb45-121">startDate</span></span>|<span data-ttu-id="cfb45-122">Date</span><span class="sxs-lookup"><span data-stu-id="cfb45-122">Date</span></span>|<span data-ttu-id="cfb45-123">Anfang des Zeitraums</span><span class="sxs-lookup"><span data-stu-id="cfb45-123">Start of the term.</span></span>|
|<span data-ttu-id="cfb45-124">endDate</span><span class="sxs-lookup"><span data-stu-id="cfb45-124">endDate</span></span>|<span data-ttu-id="cfb45-125">Date</span><span class="sxs-lookup"><span data-stu-id="cfb45-125">Date</span></span>|<span data-ttu-id="cfb45-126">Ende des Zeitraums</span><span class="sxs-lookup"><span data-stu-id="cfb45-126">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cfb45-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cfb45-127">JSON representation</span></span>

<span data-ttu-id="cfb45-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cfb45-128">The following is a JSON representation of the resource.</span></span>

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
