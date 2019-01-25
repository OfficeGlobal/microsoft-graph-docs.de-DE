---
title: Ressourcentyp educationAssignmentPointsGradeType
description: Mit der **assignments.grading** -Eigenschaft verwendet. Dies ist eine Unterklasse der EducationAssignmentGradeType.
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 567bff38f8a20456dffffdd91775a1e32852fe20
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508895"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a><span data-ttu-id="45163-104">Ressourcentyp educationAssignmentPointsGradeType</span><span class="sxs-lookup"><span data-stu-id="45163-104">educationAssignmentPointsGradeType resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45163-105">Mit der **assignments.grading** -Eigenschaft verwendet.</span><span class="sxs-lookup"><span data-stu-id="45163-105">Used with the **assignments.grading** property.</span></span> <span data-ttu-id="45163-106">Dies ist eine Unterklasse der [EducationAssignmentGradeType](educationassignmentgradetype.md).</span><span class="sxs-lookup"><span data-stu-id="45163-106">This is a subclass of [educationAssignmentGradeType](educationassignmentgradetype.md).</span></span>

<span data-ttu-id="45163-107">Dies gibt an, dass die Zuordnung bewertet ist und speichert die maximale Anzahl von Punkten, die Studenten erreichen kann auf diese Arbeitsaufgabe.</span><span class="sxs-lookup"><span data-stu-id="45163-107">This indicates that the assignment is graded and stores the maximum number of points each student can achieve on this work item.</span></span> <span data-ttu-id="45163-108">Wenn dies an einer Zuordnung festgelegt ist, erhält jede Übermittlung eine [EducationAssignmentPointsGrade](educationassignmentpointsgrade.md) -Eigenschaft für das Speichern von jeder Student Punkt zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="45163-108">When this is set on an assignment, each submission will get an [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) property associated with it for the storage of each student's points.</span></span>

## <a name="properties"></a><span data-ttu-id="45163-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="45163-109">Properties</span></span>
| <span data-ttu-id="45163-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="45163-110">Property</span></span>     | <span data-ttu-id="45163-111">Typ</span><span class="sxs-lookup"><span data-stu-id="45163-111">Type</span></span>   |<span data-ttu-id="45163-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="45163-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="45163-113">maxPoints</span><span class="sxs-lookup"><span data-stu-id="45163-113">maxPoints</span></span>|<span data-ttu-id="45163-114">Einzel</span><span class="sxs-lookup"><span data-stu-id="45163-114">Single</span></span>| <span data-ttu-id="45163-115">Max Punkte mögliche für diese Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="45163-115">Max points possible for this assignment.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="45163-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="45163-116">JSON representation</span></span>

<span data-ttu-id="45163-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="45163-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentPointsGradeType"
}-->

```json
{
  "maxPoints": "Single"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGradeType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentpointsgradetype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
