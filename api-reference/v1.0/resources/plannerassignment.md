---
title: plannerAssignment-Ressourcentyp
description: Die Ressource **PlannerAssignment** stellt die Zuordnung eines Vorgangs an einen Benutzer. Dieser Typ wird in der offenen Typ PlannerAssignments verwendet.
ms.openlocfilehash: 4fe44f39428fc8940514e68443fef072bd6d0d55
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017364"
---
# <a name="plannerassignment-resource-type"></a><span data-ttu-id="bea2e-104">plannerAssignment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bea2e-104">plannerAssignment resource type</span></span>

<span data-ttu-id="bea2e-p102">Die **plannerAssignment**-Ressource stellt die Zuweisung einer Aufgabe zu einem Benutzer dar. Dieser Typ wird im offenen Typ [plannerAssignments](plannerassignments.md) verwendet.</span><span class="sxs-lookup"><span data-stu-id="bea2e-p102">The **plannerAssignment** resource represents the assignment of a task to a user. This type is used in the open type [plannerAssignments](plannerassignments.md).</span></span>


## <a name="properties"></a><span data-ttu-id="bea2e-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bea2e-107">Properties</span></span>
| <span data-ttu-id="bea2e-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bea2e-108">Property</span></span>     | <span data-ttu-id="bea2e-109">Typ</span><span class="sxs-lookup"><span data-stu-id="bea2e-109">Type</span></span>   |<span data-ttu-id="bea2e-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bea2e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bea2e-111">assignedBy</span><span class="sxs-lookup"><span data-stu-id="bea2e-111">assignedBy</span></span>|[<span data-ttu-id="bea2e-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="bea2e-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="bea2e-113">Die Identität des Benutzers, der die Zuweisung der Aufgabe durchgeführt hat, d. h. der Zuweisende.</span><span class="sxs-lookup"><span data-stu-id="bea2e-113">The identity of the user that performed the assignment of the task, i.e. the assignor.</span></span>|
|<span data-ttu-id="bea2e-114">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="bea2e-114">assignedDateTime</span></span>|<span data-ttu-id="bea2e-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bea2e-115">DateTimeOffset</span></span>|<span data-ttu-id="bea2e-p103">Uhrzeit, zu der die Aufgabe zugewiesen wurde. Der Zeitstempeltyp stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="bea2e-p103">The time at which the task was assigned. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="bea2e-119">orderHint</span><span class="sxs-lookup"><span data-stu-id="bea2e-119">orderHint</span></span>|<span data-ttu-id="bea2e-120">String</span><span class="sxs-lookup"><span data-stu-id="bea2e-120">String</span></span>|<span data-ttu-id="bea2e-p104">Hinweis, der verwendet wird, um zugewiesene Personen in einer Aufgabe anzuordnen. Das Format ist wie [hier](planner-order-hint-format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="bea2e-p104">Hint used to order assignees in a task. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bea2e-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bea2e-123">JSON representation</span></span>
<span data-ttu-id="bea2e-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bea2e-124">Here is a JSON representation of the resource.</span></span>

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