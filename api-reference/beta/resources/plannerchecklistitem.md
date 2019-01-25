---
title: plannerChecklistItem-Ressourcentyp
description: Die **plannerChecklistItem**-Ressource stellt ein Element in der Checkliste einer Aufgabe dar. Die Checkliste für eine Aufgabe wird durch das checklistItems-Objekt dargestellt.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 87f7349e20245068a0a29a179ddb5505cd3be0ec
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522539"
---
# <a name="plannerchecklistitem-resource-type"></a><span data-ttu-id="2e9af-104">plannerChecklistItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2e9af-104">plannerChecklistItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e9af-p102">Die **plannerChecklistItem**-Ressource stellt ein Element in der Checkliste einer Aufgabe dar. Die Checkliste für eine Aufgabe wird durch das [checklistItems-Objekt](plannerchecklistitems.md) dargestellt.</span><span class="sxs-lookup"><span data-stu-id="2e9af-p102">The **plannerChecklistItem** resource represents an item in the checklist of a task. The checklist on a task is represented by the [checklistItems object](plannerchecklistitems.md).</span></span>


## <a name="properties"></a><span data-ttu-id="2e9af-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2e9af-107">Properties</span></span>
| <span data-ttu-id="2e9af-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2e9af-108">Property</span></span>     | <span data-ttu-id="2e9af-109">Typ</span><span class="sxs-lookup"><span data-stu-id="2e9af-109">Type</span></span>   |<span data-ttu-id="2e9af-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2e9af-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e9af-111">isChecked</span><span class="sxs-lookup"><span data-stu-id="2e9af-111">isChecked</span></span>|<span data-ttu-id="2e9af-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e9af-112">Boolean</span></span>|<span data-ttu-id="2e9af-113">Der Wert ist `true`, wenn das Element geprüft wurde, andernfalls `false`.</span><span class="sxs-lookup"><span data-stu-id="2e9af-113">Value is `true` if the item is checked and `false` otherwise.</span></span>|
|<span data-ttu-id="2e9af-114">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="2e9af-114">lastModifiedBy</span></span>|[<span data-ttu-id="2e9af-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="2e9af-115">identitySet</span></span>](identityset.md)| <span data-ttu-id="2e9af-p103">Schreibgeschützt. Benutzer-ID, von der das Objekt zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="2e9af-p103">Read-only. User ID by which this is last modified.</span></span>|
|<span data-ttu-id="2e9af-118">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2e9af-118">lastModifiedDateTime</span></span>|<span data-ttu-id="2e9af-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e9af-119">DateTimeOffset</span></span>|<span data-ttu-id="2e9af-p104">Schreibgeschützt. Datum und Uhrzeit der letzten Änderung des Objekts. Der Zeitstempeltyp stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2e9af-p104">Read-only. Date and time at which this is last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="2e9af-124">orderHint</span><span class="sxs-lookup"><span data-stu-id="2e9af-124">orderHint</span></span>|<span data-ttu-id="2e9af-125">String</span><span class="sxs-lookup"><span data-stu-id="2e9af-125">String</span></span>|<span data-ttu-id="2e9af-p105">Wird verwendet, um die relative Reihenfolge der Elemente in der Checkliste festzulegen. Das Format ist wie [hier](planner-order-hint-format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="2e9af-p105">Used to set the relative order of items in the checklist. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="2e9af-128">title</span><span class="sxs-lookup"><span data-stu-id="2e9af-128">title</span></span>|<span data-ttu-id="2e9af-129">String</span><span class="sxs-lookup"><span data-stu-id="2e9af-129">String</span></span>|<span data-ttu-id="2e9af-130">Titel des Checklistenelements.</span><span class="sxs-lookup"><span data-stu-id="2e9af-130">Title of the checklist item</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2e9af-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2e9af-131">JSON representation</span></span>
<span data-ttu-id="2e9af-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2e9af-132">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerChecklistItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerchecklistitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
