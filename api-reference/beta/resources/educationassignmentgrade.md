---
title: Ressourcentyp educationAssignmentGrade
description: " alle Typen von Benotung (Punkt, bestanden wurden oder usw.) werden jedoch Unterklassen dieses"
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 5ca13ba057ef000a468d910d49288d9ae8e0c962
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527857"
---
# <a name="educationassignmentgrade-resource-type"></a><span data-ttu-id="d46ae-103">Ressourcentyp educationAssignmentGrade</span><span class="sxs-lookup"><span data-stu-id="d46ae-103">educationAssignmentGrade resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d46ae-104">Stellt das **Note** -Objekt in einer Übermittlung an.</span><span class="sxs-lookup"><span data-stu-id="d46ae-104">Represents the **Grade** object on a Submission.</span></span> <span data-ttu-id="d46ae-105">Dies ist ein abstrakter Typ, der nie instanziiert wird. alle Typen von Benotung (Punkt, bestanden wurden oder usw.) werden jedoch Unterklassen dieses Typs Ressource.</span><span class="sxs-lookup"><span data-stu-id="d46ae-105">This is an abstract type that will never be instantiated; however, all types of grading (points, pass/fail, and so on) are subclasses of this resource type.</span></span> <span data-ttu-id="d46ae-106">Dieses Objekt wird auch nachverfolgt, die die Benotung Aufgaben verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="d46ae-106">This object also tracks who is doing the grading.</span></span> <span data-ttu-id="d46ae-107">In der **submission.grade** -Eigenschaft wird verwendet.</span><span class="sxs-lookup"><span data-stu-id="d46ae-107">This is used in the **submission.grade** property.</span></span>


## <a name="properties"></a><span data-ttu-id="d46ae-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d46ae-108">Properties</span></span>
| <span data-ttu-id="d46ae-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d46ae-109">Property</span></span>     | <span data-ttu-id="d46ae-110">Typ</span><span class="sxs-lookup"><span data-stu-id="d46ae-110">Type</span></span>   |<span data-ttu-id="d46ae-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d46ae-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d46ae-112">gradedBy</span><span class="sxs-lookup"><span data-stu-id="d46ae-112">gradedBy</span></span>|[<span data-ttu-id="d46ae-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="d46ae-113">identitySet</span></span>](identityset.md)| <span data-ttu-id="d46ae-114">Benutzer, der die Benotung haben.</span><span class="sxs-lookup"><span data-stu-id="d46ae-114">User who did the grading.</span></span> |
|<span data-ttu-id="d46ae-115">gradedDateTime</span><span class="sxs-lookup"><span data-stu-id="d46ae-115">gradedDateTime</span></span>|<span data-ttu-id="d46ae-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d46ae-116">DateTimeOffset</span></span>| <span data-ttu-id="d46ae-117">Zeitpunkt Uhrzeit auf dieses Objekt zum Absenden die Klasse angewendet wurde.</span><span class="sxs-lookup"><span data-stu-id="d46ae-117">Moment in time when the grade was applied to this submission object.</span></span> <span data-ttu-id="d46ae-118">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="d46ae-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d46ae-119">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d46ae-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d46ae-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d46ae-120">JSON representation</span></span>

<span data-ttu-id="d46ae-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d46ae-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentGrade"
}-->

```json
{
  "gradedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "gradedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentgrade.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
