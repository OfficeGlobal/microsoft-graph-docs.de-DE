---
title: plannerChecklistItem-Ressourcentyp
description: Die Ressource **PlannerChecklistItem** stellt ein Element in der Prüfliste eines Vorgangs dar. Die Checkliste für einen Vorgang wird durch das ChecklistItems-Objekt dargestellt.
localization_priority: Normal
ms.openlocfilehash: 116d85ecfad403409933ea485c71dd0f1ebeae9b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866479"
---
# <a name="plannerchecklistitem-resource-type"></a><span data-ttu-id="ebb52-104">plannerChecklistItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ebb52-104">plannerChecklistItem resource type</span></span>

> <span data-ttu-id="ebb52-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ebb52-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ebb52-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ebb52-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ebb52-p103">Die **plannerChecklistItem**-Ressource stellt ein Element in der Checkliste einer Aufgabe dar. Die Checkliste für eine Aufgabe wird durch das [checklistItems-Objekt](plannerchecklistitems.md) dargestellt.</span><span class="sxs-lookup"><span data-stu-id="ebb52-p103">The **plannerChecklistItem** resource represents an item in the checklist of a task. The checklist on a task is represented by the [checklistItems object](plannerchecklistitems.md).</span></span>


## <a name="properties"></a><span data-ttu-id="ebb52-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ebb52-109">Properties</span></span>
| <span data-ttu-id="ebb52-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ebb52-110">Property</span></span>     | <span data-ttu-id="ebb52-111">Typ</span><span class="sxs-lookup"><span data-stu-id="ebb52-111">Type</span></span>   |<span data-ttu-id="ebb52-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ebb52-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ebb52-113">isChecked</span><span class="sxs-lookup"><span data-stu-id="ebb52-113">isChecked</span></span>|<span data-ttu-id="ebb52-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebb52-114">Boolean</span></span>|<span data-ttu-id="ebb52-115">Der Wert ist `true`, wenn das Element geprüft wurde, andernfalls `false`.</span><span class="sxs-lookup"><span data-stu-id="ebb52-115">Value is `true` if the item is checked and `false` otherwise.</span></span>|
|<span data-ttu-id="ebb52-116">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ebb52-116">lastModifiedBy</span></span>|[<span data-ttu-id="ebb52-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="ebb52-117">identitySet</span></span>](identityset.md)| <span data-ttu-id="ebb52-p104">Schreibgeschützt. Benutzer-ID, von der das Objekt zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="ebb52-p104">Read-only. User ID by which this is last modified.</span></span>|
|<span data-ttu-id="ebb52-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ebb52-120">lastModifiedDateTime</span></span>|<span data-ttu-id="ebb52-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebb52-121">DateTimeOffset</span></span>|<span data-ttu-id="ebb52-p105">Schreibgeschützt. Datum und Uhrzeit der letzten Änderung des Objekts. Der Zeitstempeltyp stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ebb52-p105">Read-only. Date and time at which this is last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ebb52-126">orderHint</span><span class="sxs-lookup"><span data-stu-id="ebb52-126">orderHint</span></span>|<span data-ttu-id="ebb52-127">String</span><span class="sxs-lookup"><span data-stu-id="ebb52-127">String</span></span>|<span data-ttu-id="ebb52-p106">Wird verwendet, um die relative Reihenfolge der Elemente in der Checkliste festzulegen. Das Format ist wie [hier](planner-order-hint-format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="ebb52-p106">Used to set the relative order of items in the checklist. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="ebb52-130">title</span><span class="sxs-lookup"><span data-stu-id="ebb52-130">title</span></span>|<span data-ttu-id="ebb52-131">String</span><span class="sxs-lookup"><span data-stu-id="ebb52-131">String</span></span>|<span data-ttu-id="ebb52-132">Titel des Checklistenelements.</span><span class="sxs-lookup"><span data-stu-id="ebb52-132">Title of the checklist item</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ebb52-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ebb52-133">JSON representation</span></span>
<span data-ttu-id="ebb52-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ebb52-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerChecklistItem"
}-->

```json
{
  "isChecked": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "orderHint": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerChecklistItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
