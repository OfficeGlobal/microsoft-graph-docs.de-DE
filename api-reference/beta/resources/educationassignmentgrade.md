---
title: Ressourcentyp educationAssignmentGrade
description: " alle Typen von Benotung (Punkt, bestanden wurden oder usw.) werden jedoch Unterklassen dieses"
localization_priority: Normal
ms.openlocfilehash: 371346c6ff23623a118b9ee169e563e75e2429f9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889012"
---
# <a name="educationassignmentgrade-resource-type"></a><span data-ttu-id="fa88b-103">Ressourcentyp educationAssignmentGrade</span><span class="sxs-lookup"><span data-stu-id="fa88b-103">educationAssignmentGrade resource type</span></span>

> <span data-ttu-id="fa88b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fa88b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa88b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fa88b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fa88b-106">Stellt das **Note** -Objekt in einer Übermittlung an.</span><span class="sxs-lookup"><span data-stu-id="fa88b-106">Represents the **Grade** object on a Submission.</span></span> <span data-ttu-id="fa88b-107">Dies ist ein abstrakter Typ, der nie instanziiert wird. alle Typen von Benotung (Punkt, bestanden wurden oder usw.) werden jedoch Unterklassen dieses Typs Ressource.</span><span class="sxs-lookup"><span data-stu-id="fa88b-107">This is an abstract type that will never be instantiated; however, all types of grading (points, pass/fail, and so on) are subclasses of this resource type.</span></span> <span data-ttu-id="fa88b-108">Dieses Objekt wird auch nachverfolgt, die die Benotung Aufgaben verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="fa88b-108">This object also tracks who is doing the grading.</span></span> <span data-ttu-id="fa88b-109">In der **submission.grade** -Eigenschaft wird verwendet.</span><span class="sxs-lookup"><span data-stu-id="fa88b-109">This is used in the **submission.grade** property.</span></span>


## <a name="properties"></a><span data-ttu-id="fa88b-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fa88b-110">Properties</span></span>
| <span data-ttu-id="fa88b-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fa88b-111">Property</span></span>     | <span data-ttu-id="fa88b-112">Typ</span><span class="sxs-lookup"><span data-stu-id="fa88b-112">Type</span></span>   |<span data-ttu-id="fa88b-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa88b-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa88b-114">gradedBy</span><span class="sxs-lookup"><span data-stu-id="fa88b-114">gradedBy</span></span>|[<span data-ttu-id="fa88b-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="fa88b-115">identitySet</span></span>](identityset.md)| <span data-ttu-id="fa88b-116">Benutzer, der die Benotung haben.</span><span class="sxs-lookup"><span data-stu-id="fa88b-116">User who did the grading.</span></span> |
|<span data-ttu-id="fa88b-117">gradedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa88b-117">gradedDateTime</span></span>|<span data-ttu-id="fa88b-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa88b-118">DateTimeOffset</span></span>| <span data-ttu-id="fa88b-119">Zeitpunkt Uhrzeit auf dieses Objekt zum Absenden die Klasse angewendet wurde.</span><span class="sxs-lookup"><span data-stu-id="fa88b-119">Moment in time when the grade was applied to this submission object.</span></span> <span data-ttu-id="fa88b-120">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="fa88b-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fa88b-121">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="fa88b-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fa88b-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fa88b-122">JSON representation</span></span>

<span data-ttu-id="fa88b-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fa88b-123">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
