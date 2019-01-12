---
title: plannerAssignment-Ressourcentyp
description: Die Ressource **PlannerAssignment** stellt die Zuordnung eines Vorgangs an einen Benutzer. Dieser Typ wird in der offenen Typ PlannerAssignments verwendet.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 5eaeb00abf7446db1085a7c0d0916b0a7b5b2434
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963962"
---
# <a name="plannerassignment-resource-type"></a><span data-ttu-id="9a0b2-104">plannerAssignment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9a0b2-104">plannerAssignment resource type</span></span>

> <span data-ttu-id="9a0b2-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9a0b2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9a0b2-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9a0b2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9a0b2-p103">Die **plannerAssignment**-Ressource stellt die Zuweisung einer Aufgabe zu einem Benutzer dar. Dieser Typ wird im offenen Typ [plannerAssignments](plannerassignments.md) verwendet.</span><span class="sxs-lookup"><span data-stu-id="9a0b2-p103">The **plannerAssignment** resource represents the assignment of a task to a user. This type is used in the open type [plannerAssignments](plannerassignments.md).</span></span>


## <a name="properties"></a><span data-ttu-id="9a0b2-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9a0b2-109">Properties</span></span>
| <span data-ttu-id="9a0b2-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9a0b2-110">Property</span></span>     | <span data-ttu-id="9a0b2-111">Typ</span><span class="sxs-lookup"><span data-stu-id="9a0b2-111">Type</span></span>   |<span data-ttu-id="9a0b2-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9a0b2-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a0b2-113">assignedBy</span><span class="sxs-lookup"><span data-stu-id="9a0b2-113">assignedBy</span></span>|[<span data-ttu-id="9a0b2-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="9a0b2-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="9a0b2-115">Die Identität des Benutzers, der die Zuweisung der Aufgabe durchgeführt hat, d. h. der Zuweisende.</span><span class="sxs-lookup"><span data-stu-id="9a0b2-115">The identity of the user that performed the assignment of the task, i.e. the assignor.</span></span>|
|<span data-ttu-id="9a0b2-116">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a0b2-116">assignedDateTime</span></span>|<span data-ttu-id="9a0b2-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a0b2-117">DateTimeOffset</span></span>|<span data-ttu-id="9a0b2-p104">Uhrzeit, zu der die Aufgabe zugewiesen wurde. Der Zeitstempeltyp stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9a0b2-p104">The time at which the task was assigned. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9a0b2-121">orderHint</span><span class="sxs-lookup"><span data-stu-id="9a0b2-121">orderHint</span></span>|<span data-ttu-id="9a0b2-122">String</span><span class="sxs-lookup"><span data-stu-id="9a0b2-122">String</span></span>|<span data-ttu-id="9a0b2-p105">Hinweis, der verwendet wird, um zugewiesene Personen in einer Aufgabe anzuordnen. Das Format ist wie [hier](planner-order-hint-format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="9a0b2-p105">Hint used to order assignees in a task. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9a0b2-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9a0b2-125">JSON representation</span></span>
<span data-ttu-id="9a0b2-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9a0b2-126">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAssignment"
}-->

```json
{
  "assignedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "assignedDateTime": "String (timestamp)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
