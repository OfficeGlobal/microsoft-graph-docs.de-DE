---
title: Ressourcentyp pivotTable
description: Stellt eine Excel-PivotTable dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: fc43bf160e93e354ff58b2f960e8ec38d252287f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520459"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="acfd0-103">Ressourcentyp pivotTable</span><span class="sxs-lookup"><span data-stu-id="acfd0-103">pivotTable resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acfd0-104">Stellt eine Excel-PivotTable dar.</span><span class="sxs-lookup"><span data-stu-id="acfd0-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="acfd0-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="acfd0-105">Methods</span></span>

| <span data-ttu-id="acfd0-106">Methode</span><span class="sxs-lookup"><span data-stu-id="acfd0-106">Method</span></span>           | <span data-ttu-id="acfd0-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="acfd0-107">Return Type</span></span>    |<span data-ttu-id="acfd0-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="acfd0-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="acfd0-109">workbookPivotTable abrufen</span><span class="sxs-lookup"><span data-stu-id="acfd0-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="acfd0-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="acfd0-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="acfd0-111">Dient zum Lesen der Eigenschaften und der Beziehungen des workbookPivotTable-Objekts.</span><span class="sxs-lookup"><span data-stu-id="acfd0-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="acfd0-112">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="acfd0-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="acfd0-113">Keine</span><span class="sxs-lookup"><span data-stu-id="acfd0-113">None</span></span>|<span data-ttu-id="acfd0-114">Aktualisiert die PivotTable.</span><span class="sxs-lookup"><span data-stu-id="acfd0-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="acfd0-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="acfd0-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="acfd0-116">Keine</span><span class="sxs-lookup"><span data-stu-id="acfd0-116">None</span></span>|<span data-ttu-id="acfd0-p101">Aktualisiert alle Tabellen im gegebenen Arbeitsblatt. Beachten Sie, dass diese Aktion nur für die PivotTable-Sammlung verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="acfd0-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="acfd0-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="acfd0-119">Properties</span></span>
| <span data-ttu-id="acfd0-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="acfd0-120">Property</span></span>     | <span data-ttu-id="acfd0-121">Typ</span><span class="sxs-lookup"><span data-stu-id="acfd0-121">Type</span></span>   |<span data-ttu-id="acfd0-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="acfd0-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="acfd0-123">id</span><span class="sxs-lookup"><span data-stu-id="acfd0-123">id</span></span>|<span data-ttu-id="acfd0-124">String</span><span class="sxs-lookup"><span data-stu-id="acfd0-124">String</span></span>| <span data-ttu-id="acfd0-p102">Die ID der PivotTable.   Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="acfd0-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="acfd0-127">name</span><span class="sxs-lookup"><span data-stu-id="acfd0-127">name</span></span>|<span data-ttu-id="acfd0-128">String</span><span class="sxs-lookup"><span data-stu-id="acfd0-128">String</span></span>|<span data-ttu-id="acfd0-129">Der Name der PivotTable.</span><span class="sxs-lookup"><span data-stu-id="acfd0-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="acfd0-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="acfd0-130">Relationships</span></span>
| <span data-ttu-id="acfd0-131">Beziehung</span><span class="sxs-lookup"><span data-stu-id="acfd0-131">Relationship</span></span> | <span data-ttu-id="acfd0-132">Typ</span><span class="sxs-lookup"><span data-stu-id="acfd0-132">Type</span></span>   |<span data-ttu-id="acfd0-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="acfd0-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="acfd0-134">Arbeitsblatt</span><span class="sxs-lookup"><span data-stu-id="acfd0-134">worksheet</span></span>|[<span data-ttu-id="acfd0-135">Arbeitsblatt</span><span class="sxs-lookup"><span data-stu-id="acfd0-135">worksheet</span></span>](worksheet.md)| <span data-ttu-id="acfd0-p103">Das Arbeitsblatt, das die aktuelle PivotTable enthält. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="acfd0-p103">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="acfd0-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="acfd0-138">JSON representation</span></span>
<span data-ttu-id="acfd0-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="acfd0-139">Here is a JSON representation of the resource.</span></span>

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
