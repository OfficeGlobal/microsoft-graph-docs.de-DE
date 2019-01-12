---
title: Ressourcentyp educationAssignmentPointsGradeType
description: Mit der **assignments.grading** -Eigenschaft verwendet. Dies ist eine Unterklasse der EducationAssignmentGradeType.
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: b603ccec0ddd5be5003353a5062e51554cb61c53
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952664"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a><span data-ttu-id="81297-104">Ressourcentyp educationAssignmentPointsGradeType</span><span class="sxs-lookup"><span data-stu-id="81297-104">educationAssignmentPointsGradeType resource type</span></span>

> <span data-ttu-id="81297-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="81297-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81297-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="81297-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="81297-107">Mit der **assignments.grading** -Eigenschaft verwendet.</span><span class="sxs-lookup"><span data-stu-id="81297-107">Used with the **assignments.grading** property.</span></span> <span data-ttu-id="81297-108">Dies ist eine Unterklasse der [EducationAssignmentGradeType](educationassignmentgradetype.md).</span><span class="sxs-lookup"><span data-stu-id="81297-108">This is a subclass of [educationAssignmentGradeType](educationassignmentgradetype.md).</span></span>

<span data-ttu-id="81297-109">Dies gibt an, dass die Zuordnung bewertet ist und speichert die maximale Anzahl von Punkten, die Studenten erreichen kann auf diese Arbeitsaufgabe.</span><span class="sxs-lookup"><span data-stu-id="81297-109">This indicates that the assignment is graded and stores the maximum number of points each student can achieve on this work item.</span></span> <span data-ttu-id="81297-110">Wenn dies an einer Zuordnung festgelegt ist, erhält jede Übermittlung eine [EducationAssignmentPointsGrade](educationassignmentpointsgrade.md) -Eigenschaft für das Speichern von jeder Student Punkt zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="81297-110">When this is set on an assignment, each submission will get an [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) property associated with it for the storage of each student's points.</span></span>

## <a name="properties"></a><span data-ttu-id="81297-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="81297-111">Properties</span></span>
| <span data-ttu-id="81297-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="81297-112">Property</span></span>     | <span data-ttu-id="81297-113">Typ</span><span class="sxs-lookup"><span data-stu-id="81297-113">Type</span></span>   |<span data-ttu-id="81297-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="81297-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81297-115">maxPoints</span><span class="sxs-lookup"><span data-stu-id="81297-115">maxPoints</span></span>|<span data-ttu-id="81297-116">Single</span><span class="sxs-lookup"><span data-stu-id="81297-116">Single</span></span>| <span data-ttu-id="81297-117">Max Punkte mögliche für diese Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="81297-117">Max points possible for this assignment.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="81297-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="81297-118">JSON representation</span></span>

<span data-ttu-id="81297-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="81297-119">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGradeType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
