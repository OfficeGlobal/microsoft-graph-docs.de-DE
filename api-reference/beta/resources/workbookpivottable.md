---
title: Ressourcentyp pivotTable
description: Stellt eine Excel-PivotTable dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 91035b607d8c44f2d1515e9c004abd4c2235c0ec
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950858"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="190c7-103">Ressourcentyp pivotTable</span><span class="sxs-lookup"><span data-stu-id="190c7-103">pivotTable resource type</span></span>

> <span data-ttu-id="190c7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="190c7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="190c7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="190c7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="190c7-106">Stellt eine Excel-PivotTable dar.</span><span class="sxs-lookup"><span data-stu-id="190c7-106">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="190c7-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="190c7-107">Methods</span></span>

| <span data-ttu-id="190c7-108">Methode</span><span class="sxs-lookup"><span data-stu-id="190c7-108">Method</span></span>           | <span data-ttu-id="190c7-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="190c7-109">Return Type</span></span>    |<span data-ttu-id="190c7-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="190c7-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="190c7-111">workbookPivotTable abrufen</span><span class="sxs-lookup"><span data-stu-id="190c7-111">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="190c7-112">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="190c7-112">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="190c7-113">Dient zum Lesen der Eigenschaften und der Beziehungen des workbookPivotTable-Objekts.</span><span class="sxs-lookup"><span data-stu-id="190c7-113">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="190c7-114">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="190c7-114">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="190c7-115">Keine</span><span class="sxs-lookup"><span data-stu-id="190c7-115">None</span></span>|<span data-ttu-id="190c7-116">Aktualisiert die PivotTable.</span><span class="sxs-lookup"><span data-stu-id="190c7-116">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="190c7-117">Refreshall</span><span class="sxs-lookup"><span data-stu-id="190c7-117">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="190c7-118">Keine</span><span class="sxs-lookup"><span data-stu-id="190c7-118">None</span></span>|<span data-ttu-id="190c7-p102">Aktualisiert alle Tabellen im gegebenen Arbeitsblatt. Beachten Sie, dass diese Aktion nur für die PivotTable-Sammlung verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="190c7-p102">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="190c7-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="190c7-121">Properties</span></span>
| <span data-ttu-id="190c7-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="190c7-122">Property</span></span>     | <span data-ttu-id="190c7-123">Typ</span><span class="sxs-lookup"><span data-stu-id="190c7-123">Type</span></span>   |<span data-ttu-id="190c7-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="190c7-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="190c7-125">id</span><span class="sxs-lookup"><span data-stu-id="190c7-125">id</span></span>|<span data-ttu-id="190c7-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="190c7-126">String</span></span>| <span data-ttu-id="190c7-p103">Die ID der PivotTable.   Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="190c7-p103">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="190c7-129">name</span><span class="sxs-lookup"><span data-stu-id="190c7-129">name</span></span>|<span data-ttu-id="190c7-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="190c7-130">String</span></span>|<span data-ttu-id="190c7-131">Der Name der PivotTable.</span><span class="sxs-lookup"><span data-stu-id="190c7-131">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="190c7-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="190c7-132">Relationships</span></span>
| <span data-ttu-id="190c7-133">Beziehung</span><span class="sxs-lookup"><span data-stu-id="190c7-133">Relationship</span></span> | <span data-ttu-id="190c7-134">Typ</span><span class="sxs-lookup"><span data-stu-id="190c7-134">Type</span></span>   |<span data-ttu-id="190c7-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="190c7-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="190c7-136">Arbeitsblatt</span><span class="sxs-lookup"><span data-stu-id="190c7-136">worksheet</span></span>|[<span data-ttu-id="190c7-137">Arbeitsblatt</span><span class="sxs-lookup"><span data-stu-id="190c7-137">worksheet</span></span>](worksheet.md)| <span data-ttu-id="190c7-p104">Das Arbeitsblatt, das die aktuelle PivotTable enthält. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="190c7-p104">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="190c7-140">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="190c7-140">JSON representation</span></span>
<span data-ttu-id="190c7-141">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="190c7-141">Here is a JSON representation of the resource.</span></span>

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
