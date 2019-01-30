---
title: Ressourcentyp pivotTable
description: Stellt eine Excel-PivotTable dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: fc43bf160e93e354ff58b2f960e8ec38d252287f
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641106"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="efdd5-103">Ressourcentyp pivotTable</span><span class="sxs-lookup"><span data-stu-id="efdd5-103">pivotTable resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efdd5-104">Stellt eine Excel-PivotTable dar.</span><span class="sxs-lookup"><span data-stu-id="efdd5-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="efdd5-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="efdd5-105">Methods</span></span>

| <span data-ttu-id="efdd5-106">Methode</span><span class="sxs-lookup"><span data-stu-id="efdd5-106">Method</span></span>           | <span data-ttu-id="efdd5-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="efdd5-107">Return Type</span></span>    |<span data-ttu-id="efdd5-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="efdd5-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="efdd5-109">workbookPivotTable abrufen</span><span class="sxs-lookup"><span data-stu-id="efdd5-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="efdd5-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="efdd5-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="efdd5-111">Dient zum Lesen der Eigenschaften und der Beziehungen des workbookPivotTable-Objekts.</span><span class="sxs-lookup"><span data-stu-id="efdd5-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="efdd5-112">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="efdd5-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="efdd5-113">Keine</span><span class="sxs-lookup"><span data-stu-id="efdd5-113">None</span></span>|<span data-ttu-id="efdd5-114">Aktualisiert die PivotTable.</span><span class="sxs-lookup"><span data-stu-id="efdd5-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="efdd5-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="efdd5-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="efdd5-116">Keine</span><span class="sxs-lookup"><span data-stu-id="efdd5-116">None</span></span>|<span data-ttu-id="efdd5-p101">Aktualisiert alle Tabellen im gegebenen Arbeitsblatt. Beachten Sie, dass diese Aktion nur für die PivotTable-Sammlung verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="efdd5-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="efdd5-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="efdd5-119">Properties</span></span>
| <span data-ttu-id="efdd5-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="efdd5-120">Property</span></span>     | <span data-ttu-id="efdd5-121">Typ</span><span class="sxs-lookup"><span data-stu-id="efdd5-121">Type</span></span>   |<span data-ttu-id="efdd5-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="efdd5-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="efdd5-123">id</span><span class="sxs-lookup"><span data-stu-id="efdd5-123">id</span></span>|<span data-ttu-id="efdd5-124">String</span><span class="sxs-lookup"><span data-stu-id="efdd5-124">String</span></span>| <span data-ttu-id="efdd5-p102">Die ID der PivotTable.   Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="efdd5-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="efdd5-127">name</span><span class="sxs-lookup"><span data-stu-id="efdd5-127">name</span></span>|<span data-ttu-id="efdd5-128">String</span><span class="sxs-lookup"><span data-stu-id="efdd5-128">String</span></span>|<span data-ttu-id="efdd5-129">Der Name der PivotTable.</span><span class="sxs-lookup"><span data-stu-id="efdd5-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="efdd5-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="efdd5-130">Relationships</span></span>
| <span data-ttu-id="efdd5-131">Beziehung</span><span class="sxs-lookup"><span data-stu-id="efdd5-131">Relationship</span></span> | <span data-ttu-id="efdd5-132">Typ</span><span class="sxs-lookup"><span data-stu-id="efdd5-132">Type</span></span>   |<span data-ttu-id="efdd5-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="efdd5-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="efdd5-134">Arbeitsblatt</span><span class="sxs-lookup"><span data-stu-id="efdd5-134">worksheet</span></span>|[<span data-ttu-id="efdd5-135">Arbeitsblatt</span><span class="sxs-lookup"><span data-stu-id="efdd5-135">worksheet</span></span>](worksheet.md)| <span data-ttu-id="efdd5-p103">Das Arbeitsblatt, das die aktuelle PivotTable enthält. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="efdd5-p103">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="efdd5-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="efdd5-138">JSON representation</span></span>
<span data-ttu-id="efdd5-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="efdd5-139">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookPivotTable"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/workbookpivottable.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
