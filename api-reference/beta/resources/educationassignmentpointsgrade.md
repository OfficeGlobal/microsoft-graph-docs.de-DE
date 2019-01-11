---
title: Ressourcentyp educationAssignmentPointsGrade
description: Wenn eine Zuordnung zu einem Punkt Note festgelegt ist, wird jede Übermittlung dieses Objekt die **submission.grade** -Eigenschaft zugeordnet haben. Dadurch wird eine Unterklasse von EducationAssignmentGrade,
localization_priority: Normal
ms.openlocfilehash: 2084a1bda6784165576c3ec454fa9ee88601c952
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861404"
---
# <a name="educationassignmentpointsgrade-resource-type"></a><span data-ttu-id="ad8f4-104">Ressourcentyp educationAssignmentPointsGrade</span><span class="sxs-lookup"><span data-stu-id="ad8f4-104">educationAssignmentPointsGrade resource type</span></span>

> <span data-ttu-id="ad8f4-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ad8f4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad8f4-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ad8f4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ad8f4-107">Wenn eine Zuordnung zu einem Punkt Note festgelegt ist, wird jede Übermittlung dieses Objekt die **submission.grade** -Eigenschaft zugeordnet haben.</span><span class="sxs-lookup"><span data-stu-id="ad8f4-107">When an assignment is set to a points grade type, each submission will have this object associated with the **submission.grade** property.</span></span> <span data-ttu-id="ad8f4-108">Dadurch wird eine Unterklasse von [EducationAssignmentGrade](educationassignmentgrade.md), die die, die Daten für diese Eigenschaft hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="ad8f4-108">This creates a subclass from [educationAssignmentGrade](educationassignmentgrade.md), which will add the who data to this property.</span></span> <span data-ttu-id="ad8f4-109">Die maximale Punkte in die **assignments.grading** -Eigenschaft gespeichert ist.</span><span class="sxs-lookup"><span data-stu-id="ad8f4-109">The max points is stored in the **assignments.grading** property.</span></span>


## <a name="properties"></a><span data-ttu-id="ad8f4-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ad8f4-110">Properties</span></span>
| <span data-ttu-id="ad8f4-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ad8f4-111">Property</span></span>     | <span data-ttu-id="ad8f4-112">Typ</span><span class="sxs-lookup"><span data-stu-id="ad8f4-112">Type</span></span>   |<span data-ttu-id="ad8f4-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ad8f4-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad8f4-114">points</span><span class="sxs-lookup"><span data-stu-id="ad8f4-114">points</span></span>|<span data-ttu-id="ad8f4-115">Single</span><span class="sxs-lookup"><span data-stu-id="ad8f4-115">Single</span></span>|<span data-ttu-id="ad8f4-116">Anzahl von Punkten a Lehrer ist dieses Objekt Übermittlung erteilen.</span><span class="sxs-lookup"><span data-stu-id="ad8f4-116">Number of points a teacher is giving this submission object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ad8f4-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ad8f4-117">JSON representation</span></span>

<span data-ttu-id="ad8f4-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ad8f4-118">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
