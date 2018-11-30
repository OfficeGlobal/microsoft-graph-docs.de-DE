---
title: Ressourcentyp pivotTable
description: Stellt eine Excel-PivotTable dar.
ms.openlocfilehash: b4ddd0c1bb9e4ee13aaf3d1b4472c4e750e3a755
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016676"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="845bc-103">Ressourcentyp pivotTable</span><span class="sxs-lookup"><span data-stu-id="845bc-103">pivotTable resource type</span></span>

<span data-ttu-id="845bc-104">Stellt eine Excel-PivotTable dar.</span><span class="sxs-lookup"><span data-stu-id="845bc-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="845bc-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="845bc-105">Methods</span></span>

| <span data-ttu-id="845bc-106">Methode</span><span class="sxs-lookup"><span data-stu-id="845bc-106">Method</span></span>           | <span data-ttu-id="845bc-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="845bc-107">Return Type</span></span>    |<span data-ttu-id="845bc-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="845bc-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="845bc-109">workbookPivotTable abrufen</span><span class="sxs-lookup"><span data-stu-id="845bc-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="845bc-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="845bc-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="845bc-111">Dient zum Lesen der Eigenschaften und der Beziehungen des workbookPivotTable-Objekts.</span><span class="sxs-lookup"><span data-stu-id="845bc-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="845bc-112">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="845bc-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="845bc-113">Keine</span><span class="sxs-lookup"><span data-stu-id="845bc-113">None</span></span>|<span data-ttu-id="845bc-114">Aktualisiert die PivotTable.</span><span class="sxs-lookup"><span data-stu-id="845bc-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="845bc-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="845bc-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="845bc-116">Keine</span><span class="sxs-lookup"><span data-stu-id="845bc-116">None</span></span>|<span data-ttu-id="845bc-p101">Aktualisiert alle Tabellen im gegebenen Arbeitsblatt. Beachten Sie, dass diese Aktion nur für die PivotTable-Sammlung verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="845bc-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="845bc-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="845bc-119">Properties</span></span>
| <span data-ttu-id="845bc-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="845bc-120">Property</span></span>     | <span data-ttu-id="845bc-121">Typ</span><span class="sxs-lookup"><span data-stu-id="845bc-121">Type</span></span>   |<span data-ttu-id="845bc-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="845bc-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="845bc-123">id</span><span class="sxs-lookup"><span data-stu-id="845bc-123">id</span></span>|<span data-ttu-id="845bc-124">String</span><span class="sxs-lookup"><span data-stu-id="845bc-124">String</span></span>| <span data-ttu-id="845bc-p102">Die ID der PivotTable.   Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="845bc-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="845bc-127">name</span><span class="sxs-lookup"><span data-stu-id="845bc-127">name</span></span>|<span data-ttu-id="845bc-128">String</span><span class="sxs-lookup"><span data-stu-id="845bc-128">String</span></span>|<span data-ttu-id="845bc-129">Der Name der PivotTable.</span><span class="sxs-lookup"><span data-stu-id="845bc-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="845bc-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="845bc-130">Relationships</span></span>
| <span data-ttu-id="845bc-131">Beziehung</span><span class="sxs-lookup"><span data-stu-id="845bc-131">Relationship</span></span> | <span data-ttu-id="845bc-132">Typ</span><span class="sxs-lookup"><span data-stu-id="845bc-132">Type</span></span>   |<span data-ttu-id="845bc-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="845bc-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="845bc-134">Arbeitsblatt</span><span class="sxs-lookup"><span data-stu-id="845bc-134">worksheet</span></span>|[<span data-ttu-id="845bc-135">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="845bc-135">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="845bc-p103">Das Arbeitsblatt, das die aktuelle PivotTable enthält. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="845bc-p103">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="845bc-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="845bc-138">JSON representation</span></span>
<span data-ttu-id="845bc-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="845bc-139">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
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
