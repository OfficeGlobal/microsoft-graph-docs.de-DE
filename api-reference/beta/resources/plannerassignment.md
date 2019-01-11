---
title: plannerAssignment-Ressourcentyp
description: Die Ressource **PlannerAssignment** stellt die Zuordnung eines Vorgangs an einen Benutzer. Dieser Typ wird in der offenen Typ PlannerAssignments verwendet.
localization_priority: Normal
ms.openlocfilehash: 61591a6d0181c0ce54d96b09b314c235803265c4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856042"
---
# <a name="plannerassignment-resource-type"></a><span data-ttu-id="8fafe-104">plannerAssignment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8fafe-104">plannerAssignment resource type</span></span>

> <span data-ttu-id="8fafe-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8fafe-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8fafe-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8fafe-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8fafe-p103">Die **plannerAssignment**-Ressource stellt die Zuweisung einer Aufgabe zu einem Benutzer dar. Dieser Typ wird im offenen Typ [plannerAssignments](plannerassignments.md) verwendet.</span><span class="sxs-lookup"><span data-stu-id="8fafe-p103">The **plannerAssignment** resource represents the assignment of a task to a user. This type is used in the open type [plannerAssignments](plannerassignments.md).</span></span>


## <a name="properties"></a><span data-ttu-id="8fafe-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8fafe-109">Properties</span></span>
| <span data-ttu-id="8fafe-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8fafe-110">Property</span></span>     | <span data-ttu-id="8fafe-111">Typ</span><span class="sxs-lookup"><span data-stu-id="8fafe-111">Type</span></span>   |<span data-ttu-id="8fafe-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8fafe-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8fafe-113">assignedBy</span><span class="sxs-lookup"><span data-stu-id="8fafe-113">assignedBy</span></span>|[<span data-ttu-id="8fafe-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="8fafe-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="8fafe-115">Die Identität des Benutzers, der die Zuweisung der Aufgabe durchgeführt hat, d. h. der Zuweisende.</span><span class="sxs-lookup"><span data-stu-id="8fafe-115">The identity of the user that performed the assignment of the task, i.e. the assignor.</span></span>|
|<span data-ttu-id="8fafe-116">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="8fafe-116">assignedDateTime</span></span>|<span data-ttu-id="8fafe-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fafe-117">DateTimeOffset</span></span>|<span data-ttu-id="8fafe-p104">Uhrzeit, zu der die Aufgabe zugewiesen wurde. Der Zeitstempeltyp stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="8fafe-p104">The time at which the task was assigned. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="8fafe-121">orderHint</span><span class="sxs-lookup"><span data-stu-id="8fafe-121">orderHint</span></span>|<span data-ttu-id="8fafe-122">String</span><span class="sxs-lookup"><span data-stu-id="8fafe-122">String</span></span>|<span data-ttu-id="8fafe-p105">Hinweis, der verwendet wird, um zugewiesene Personen in einer Aufgabe anzuordnen. Das Format ist wie [hier](planner-order-hint-format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="8fafe-p105">Hint used to order assignees in a task. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8fafe-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8fafe-125">JSON representation</span></span>
<span data-ttu-id="8fafe-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8fafe-126">Here is a JSON representation of the resource.</span></span>

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
