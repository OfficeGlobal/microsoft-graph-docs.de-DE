---
title: Ressourcentyp pivotTable
description: Stellt eine Excel-PivotTable dar.
ms.openlocfilehash: 3cba1263715400def6b66149ecec11eddde5e686
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064073"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="ce0cc-103">Ressourcentyp pivotTable</span><span class="sxs-lookup"><span data-stu-id="ce0cc-103">pivotTable resource type</span></span>

> <span data-ttu-id="ce0cc-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ce0cc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ce0cc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ce0cc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ce0cc-106">Stellt eine Excel-PivotTable dar.</span><span class="sxs-lookup"><span data-stu-id="ce0cc-106">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="ce0cc-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="ce0cc-107">Methods</span></span>

| <span data-ttu-id="ce0cc-108">Methode</span><span class="sxs-lookup"><span data-stu-id="ce0cc-108">Method</span></span>           | <span data-ttu-id="ce0cc-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="ce0cc-109">Return Type</span></span>    |<span data-ttu-id="ce0cc-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ce0cc-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ce0cc-111">workbookPivotTable abrufen</span><span class="sxs-lookup"><span data-stu-id="ce0cc-111">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="ce0cc-112">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="ce0cc-112">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="ce0cc-113">Dient zum Lesen der Eigenschaften und der Beziehungen des workbookPivotTable-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ce0cc-113">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="ce0cc-114">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ce0cc-114">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="ce0cc-115">Keine</span><span class="sxs-lookup"><span data-stu-id="ce0cc-115">None</span></span>|<span data-ttu-id="ce0cc-116">Aktualisiert die PivotTable.</span><span class="sxs-lookup"><span data-stu-id="ce0cc-116">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="ce0cc-117">Refreshall</span><span class="sxs-lookup"><span data-stu-id="ce0cc-117">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="ce0cc-118">Keine</span><span class="sxs-lookup"><span data-stu-id="ce0cc-118">None</span></span>|<span data-ttu-id="ce0cc-p102">Aktualisiert alle Tabellen im gegebenen Arbeitsblatt. Beachten Sie, dass diese Aktion nur für die PivotTable-Sammlung verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="ce0cc-p102">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="ce0cc-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ce0cc-121">Properties</span></span>
| <span data-ttu-id="ce0cc-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ce0cc-122">Property</span></span>     | <span data-ttu-id="ce0cc-123">Typ</span><span class="sxs-lookup"><span data-stu-id="ce0cc-123">Type</span></span>   |<span data-ttu-id="ce0cc-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ce0cc-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce0cc-125">id</span><span class="sxs-lookup"><span data-stu-id="ce0cc-125">id</span></span>|<span data-ttu-id="ce0cc-126">String</span><span class="sxs-lookup"><span data-stu-id="ce0cc-126">String</span></span>| <span data-ttu-id="ce0cc-p103">Die ID der PivotTable.   Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ce0cc-p103">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="ce0cc-129">name</span><span class="sxs-lookup"><span data-stu-id="ce0cc-129">name</span></span>|<span data-ttu-id="ce0cc-130">String</span><span class="sxs-lookup"><span data-stu-id="ce0cc-130">String</span></span>|<span data-ttu-id="ce0cc-131">Der Name der PivotTable.</span><span class="sxs-lookup"><span data-stu-id="ce0cc-131">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="ce0cc-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ce0cc-132">Relationships</span></span>
| <span data-ttu-id="ce0cc-133">Beziehung</span><span class="sxs-lookup"><span data-stu-id="ce0cc-133">Relationship</span></span> | <span data-ttu-id="ce0cc-134">Typ</span><span class="sxs-lookup"><span data-stu-id="ce0cc-134">Type</span></span>   |<span data-ttu-id="ce0cc-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ce0cc-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce0cc-136">Arbeitsblatt</span><span class="sxs-lookup"><span data-stu-id="ce0cc-136">worksheet</span></span>|[<span data-ttu-id="ce0cc-137">Arbeitsblatt</span><span class="sxs-lookup"><span data-stu-id="ce0cc-137">worksheet</span></span>](worksheet.md)| <span data-ttu-id="ce0cc-p104">Das Arbeitsblatt, das die aktuelle PivotTable enthält. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ce0cc-p104">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="ce0cc-140">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ce0cc-140">JSON representation</span></span>
<span data-ttu-id="ce0cc-141">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ce0cc-141">Here is a JSON representation of the resource.</span></span>

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
