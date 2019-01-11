---
title: Ressourcentyp pivotTable
description: Stellt eine Excel-PivotTable dar.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: d500d4bc88608b032262cfae505385bf7ed3f072
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889208"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="f9f7e-103">Ressourcentyp pivotTable</span><span class="sxs-lookup"><span data-stu-id="f9f7e-103">pivotTable resource type</span></span>

<span data-ttu-id="f9f7e-104">Stellt eine Excel-PivotTable dar.</span><span class="sxs-lookup"><span data-stu-id="f9f7e-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="f9f7e-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="f9f7e-105">Methods</span></span>

| <span data-ttu-id="f9f7e-106">Methode</span><span class="sxs-lookup"><span data-stu-id="f9f7e-106">Method</span></span>           | <span data-ttu-id="f9f7e-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="f9f7e-107">Return Type</span></span>    |<span data-ttu-id="f9f7e-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f9f7e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f9f7e-109">workbookPivotTable abrufen</span><span class="sxs-lookup"><span data-stu-id="f9f7e-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="f9f7e-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="f9f7e-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="f9f7e-111">Dient zum Lesen der Eigenschaften und der Beziehungen des workbookPivotTable-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f9f7e-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="f9f7e-112">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f9f7e-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="f9f7e-113">Keine</span><span class="sxs-lookup"><span data-stu-id="f9f7e-113">None</span></span>|<span data-ttu-id="f9f7e-114">Aktualisiert die PivotTable.</span><span class="sxs-lookup"><span data-stu-id="f9f7e-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="f9f7e-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="f9f7e-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="f9f7e-116">Keine</span><span class="sxs-lookup"><span data-stu-id="f9f7e-116">None</span></span>|<span data-ttu-id="f9f7e-p101">Aktualisiert alle Tabellen im gegebenen Arbeitsblatt. Beachten Sie, dass diese Aktion nur für die PivotTable-Sammlung verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="f9f7e-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="f9f7e-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f9f7e-119">Properties</span></span>
| <span data-ttu-id="f9f7e-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f9f7e-120">Property</span></span>     | <span data-ttu-id="f9f7e-121">Typ</span><span class="sxs-lookup"><span data-stu-id="f9f7e-121">Type</span></span>   |<span data-ttu-id="f9f7e-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f9f7e-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9f7e-123">id</span><span class="sxs-lookup"><span data-stu-id="f9f7e-123">id</span></span>|<span data-ttu-id="f9f7e-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f9f7e-124">String</span></span>| <span data-ttu-id="f9f7e-p102">Die ID der PivotTable.   Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f9f7e-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="f9f7e-127">name</span><span class="sxs-lookup"><span data-stu-id="f9f7e-127">name</span></span>|<span data-ttu-id="f9f7e-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f9f7e-128">String</span></span>|<span data-ttu-id="f9f7e-129">Der Name der PivotTable.</span><span class="sxs-lookup"><span data-stu-id="f9f7e-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="f9f7e-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f9f7e-130">Relationships</span></span>
| <span data-ttu-id="f9f7e-131">Beziehung</span><span class="sxs-lookup"><span data-stu-id="f9f7e-131">Relationship</span></span> | <span data-ttu-id="f9f7e-132">Typ</span><span class="sxs-lookup"><span data-stu-id="f9f7e-132">Type</span></span>   |<span data-ttu-id="f9f7e-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f9f7e-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9f7e-134">Arbeitsblatt</span><span class="sxs-lookup"><span data-stu-id="f9f7e-134">worksheet</span></span>|[<span data-ttu-id="f9f7e-135">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="f9f7e-135">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="f9f7e-p103">Das Arbeitsblatt, das die aktuelle PivotTable enthält. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f9f7e-p103">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="f9f7e-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f9f7e-138">JSON representation</span></span>
<span data-ttu-id="f9f7e-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f9f7e-139">Here is a JSON representation of the resource.</span></span>

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
