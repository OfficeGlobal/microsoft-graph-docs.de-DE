---
title: Ressourcentyp pivotTable
description: Stellt eine Excel-PivotTable dar.
author: lumine2008
ms.openlocfilehash: 68075aebeac9c0846e48739daf65e5bf97e4d6f5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334111"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="71364-103">Ressourcentyp pivotTable</span><span class="sxs-lookup"><span data-stu-id="71364-103">pivotTable resource type</span></span>

<span data-ttu-id="71364-104">Stellt eine Excel-PivotTable dar.</span><span class="sxs-lookup"><span data-stu-id="71364-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="71364-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="71364-105">Methods</span></span>

| <span data-ttu-id="71364-106">Methode</span><span class="sxs-lookup"><span data-stu-id="71364-106">Method</span></span>           | <span data-ttu-id="71364-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="71364-107">Return Type</span></span>    |<span data-ttu-id="71364-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71364-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="71364-109">workbookPivotTable abrufen</span><span class="sxs-lookup"><span data-stu-id="71364-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="71364-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="71364-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="71364-111">Dient zum Lesen der Eigenschaften und der Beziehungen des workbookPivotTable-Objekts.</span><span class="sxs-lookup"><span data-stu-id="71364-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="71364-112">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="71364-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="71364-113">Keine</span><span class="sxs-lookup"><span data-stu-id="71364-113">None</span></span>|<span data-ttu-id="71364-114">Aktualisiert die PivotTable.</span><span class="sxs-lookup"><span data-stu-id="71364-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="71364-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="71364-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="71364-116">Keine</span><span class="sxs-lookup"><span data-stu-id="71364-116">None</span></span>|<span data-ttu-id="71364-p101">Aktualisiert alle Tabellen im gegebenen Arbeitsblatt. Beachten Sie, dass diese Aktion nur für die PivotTable-Sammlung verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="71364-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="71364-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="71364-119">Properties</span></span>
| <span data-ttu-id="71364-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="71364-120">Property</span></span>     | <span data-ttu-id="71364-121">Typ</span><span class="sxs-lookup"><span data-stu-id="71364-121">Type</span></span>   |<span data-ttu-id="71364-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71364-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71364-123">id</span><span class="sxs-lookup"><span data-stu-id="71364-123">id</span></span>|<span data-ttu-id="71364-124">String</span><span class="sxs-lookup"><span data-stu-id="71364-124">String</span></span>| <span data-ttu-id="71364-p102">Die ID der PivotTable.   Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="71364-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="71364-127">name</span><span class="sxs-lookup"><span data-stu-id="71364-127">name</span></span>|<span data-ttu-id="71364-128">String</span><span class="sxs-lookup"><span data-stu-id="71364-128">String</span></span>|<span data-ttu-id="71364-129">Der Name der PivotTable.</span><span class="sxs-lookup"><span data-stu-id="71364-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="71364-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="71364-130">Relationships</span></span>
| <span data-ttu-id="71364-131">Beziehung</span><span class="sxs-lookup"><span data-stu-id="71364-131">Relationship</span></span> | <span data-ttu-id="71364-132">Typ</span><span class="sxs-lookup"><span data-stu-id="71364-132">Type</span></span>   |<span data-ttu-id="71364-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71364-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71364-134">Arbeitsblatt</span><span class="sxs-lookup"><span data-stu-id="71364-134">worksheet</span></span>|[<span data-ttu-id="71364-135">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="71364-135">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="71364-p103">Das Arbeitsblatt, das die aktuelle PivotTable enthält. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="71364-p103">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="71364-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="71364-138">JSON representation</span></span>
<span data-ttu-id="71364-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="71364-139">Here is a JSON representation of the resource.</span></span>

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
