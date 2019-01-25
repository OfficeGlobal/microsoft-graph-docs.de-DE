---
title: plannerAssignment-Ressourcentyp
description: Die **plannerAssignment**-Ressource stellt die Zuweisung einer Aufgabe zu einem Benutzer dar. Dieser Typ wird im offenen Typ plannerAssignments verwendet.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 054cd42eedd27a7fe11abc2e5578a56da667e05d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522504"
---
# <a name="plannerassignment-resource-type"></a><span data-ttu-id="df6e2-104">plannerAssignment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="df6e2-104">plannerAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df6e2-p102">Die **plannerAssignment**-Ressource stellt die Zuweisung einer Aufgabe zu einem Benutzer dar. Dieser Typ wird im offenen Typ [plannerAssignments](plannerassignments.md) verwendet.</span><span class="sxs-lookup"><span data-stu-id="df6e2-p102">The **plannerAssignment** resource represents the assignment of a task to a user. This type is used in the open type [plannerAssignments](plannerassignments.md).</span></span>


## <a name="properties"></a><span data-ttu-id="df6e2-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="df6e2-107">Properties</span></span>
| <span data-ttu-id="df6e2-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="df6e2-108">Property</span></span>     | <span data-ttu-id="df6e2-109">Typ</span><span class="sxs-lookup"><span data-stu-id="df6e2-109">Type</span></span>   |<span data-ttu-id="df6e2-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="df6e2-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="df6e2-111">assignedBy</span><span class="sxs-lookup"><span data-stu-id="df6e2-111">assignedBy</span></span>|[<span data-ttu-id="df6e2-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="df6e2-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="df6e2-113">Die Identität des Benutzers, der die Zuweisung der Aufgabe durchgeführt hat, d. h. der Zuweisende.</span><span class="sxs-lookup"><span data-stu-id="df6e2-113">The identity of the user that performed the assignment of the task, i.e. the assignor.</span></span>|
|<span data-ttu-id="df6e2-114">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="df6e2-114">assignedDateTime</span></span>|<span data-ttu-id="df6e2-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df6e2-115">DateTimeOffset</span></span>|<span data-ttu-id="df6e2-p103">Uhrzeit, zu der die Aufgabe zugewiesen wurde. Der Zeitstempeltyp stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="df6e2-p103">The time at which the task was assigned. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="df6e2-119">orderHint</span><span class="sxs-lookup"><span data-stu-id="df6e2-119">orderHint</span></span>|<span data-ttu-id="df6e2-120">String</span><span class="sxs-lookup"><span data-stu-id="df6e2-120">String</span></span>|<span data-ttu-id="df6e2-p104">Hinweis, der verwendet wird, um zugewiesene Personen in einer Aufgabe anzuordnen. Das Format ist wie [hier](planner-order-hint-format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="df6e2-p104">Hint used to order assignees in a task. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="df6e2-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="df6e2-123">JSON representation</span></span>
<span data-ttu-id="df6e2-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="df6e2-124">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
