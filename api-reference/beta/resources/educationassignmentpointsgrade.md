---
title: Ressourcentyp educationAssignmentPointsGrade
description: Wenn eine Zuordnung zu einem Punkt Note festgelegt ist, wird jede Übermittlung dieses Objekt die **submission.grade** -Eigenschaft zugeordnet haben. Dadurch wird eine Unterklasse von EducationAssignmentGrade,
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 5d2a5cf6f6f886185179c6f1a61c1bb1d9d1ecfc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523736"
---
# <a name="educationassignmentpointsgrade-resource-type"></a><span data-ttu-id="6d2e4-104">Ressourcentyp educationAssignmentPointsGrade</span><span class="sxs-lookup"><span data-stu-id="6d2e4-104">educationAssignmentPointsGrade resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d2e4-105">Wenn eine Zuordnung zu einem Punkt Note festgelegt ist, wird jede Übermittlung dieses Objekt die **submission.grade** -Eigenschaft zugeordnet haben.</span><span class="sxs-lookup"><span data-stu-id="6d2e4-105">When an assignment is set to a points grade type, each submission will have this object associated with the **submission.grade** property.</span></span> <span data-ttu-id="6d2e4-106">Dadurch wird eine Unterklasse von [EducationAssignmentGrade](educationassignmentgrade.md), die die, die Daten für diese Eigenschaft hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="6d2e4-106">This creates a subclass from [educationAssignmentGrade](educationassignmentgrade.md), which will add the who data to this property.</span></span> <span data-ttu-id="6d2e4-107">Die maximale Punkte in die **assignments.grading** -Eigenschaft gespeichert ist.</span><span class="sxs-lookup"><span data-stu-id="6d2e4-107">The max points is stored in the **assignments.grading** property.</span></span>


## <a name="properties"></a><span data-ttu-id="6d2e4-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6d2e4-108">Properties</span></span>
| <span data-ttu-id="6d2e4-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6d2e4-109">Property</span></span>     | <span data-ttu-id="6d2e4-110">Typ</span><span class="sxs-lookup"><span data-stu-id="6d2e4-110">Type</span></span>   |<span data-ttu-id="6d2e4-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6d2e4-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d2e4-112">points</span><span class="sxs-lookup"><span data-stu-id="6d2e4-112">points</span></span>|<span data-ttu-id="6d2e4-113">Einzel</span><span class="sxs-lookup"><span data-stu-id="6d2e4-113">Single</span></span>|<span data-ttu-id="6d2e4-114">Anzahl von Punkten a Lehrer ist dieses Objekt Übermittlung erteilen.</span><span class="sxs-lookup"><span data-stu-id="6d2e4-114">Number of points a teacher is giving this submission object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6d2e4-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6d2e4-115">JSON representation</span></span>

<span data-ttu-id="6d2e4-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6d2e4-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentPointsGrade"
}-->

```json
{
  "points": "Single"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentpointsgrade.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
