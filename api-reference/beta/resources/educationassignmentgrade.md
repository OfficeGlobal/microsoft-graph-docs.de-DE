---
title: Ressourcentyp educationAssignmentGrade
description: " alle Typen von Benotung (Punkt, bestanden wurden oder usw.) werden jedoch Unterklassen dieses"
ms.openlocfilehash: c9cd043f8887fda9427d7b56cf832001361d03a9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063543"
---
# <a name="educationassignmentgrade-resource-type"></a><span data-ttu-id="f8fb0-103">Ressourcentyp educationAssignmentGrade</span><span class="sxs-lookup"><span data-stu-id="f8fb0-103">educationAssignmentGrade resource type</span></span>

> <span data-ttu-id="f8fb0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f8fb0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8fb0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f8fb0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f8fb0-106">Stellt das **Note** -Objekt in einer Übermittlung an.</span><span class="sxs-lookup"><span data-stu-id="f8fb0-106">Represents the **Grade** object on a Submission.</span></span> <span data-ttu-id="f8fb0-107">Dies ist ein abstrakter Typ, der nie instanziiert wird. alle Typen von Benotung (Punkt, bestanden wurden oder usw.) werden jedoch Unterklassen dieses Typs Ressource.</span><span class="sxs-lookup"><span data-stu-id="f8fb0-107">This is an abstract type that will never be instantiated; however, all types of grading (points, pass/fail, and so on) are subclasses of this resource type.</span></span> <span data-ttu-id="f8fb0-108">Dieses Objekt wird auch nachverfolgt, die die Benotung Aufgaben verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="f8fb0-108">This object also tracks who is doing the grading.</span></span> <span data-ttu-id="f8fb0-109">In der **submission.grade** -Eigenschaft wird verwendet.</span><span class="sxs-lookup"><span data-stu-id="f8fb0-109">This is used in the **submission.grade** property.</span></span>


## <a name="properties"></a><span data-ttu-id="f8fb0-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f8fb0-110">Properties</span></span>
| <span data-ttu-id="f8fb0-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f8fb0-111">Property</span></span>     | <span data-ttu-id="f8fb0-112">Typ</span><span class="sxs-lookup"><span data-stu-id="f8fb0-112">Type</span></span>   |<span data-ttu-id="f8fb0-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8fb0-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f8fb0-114">gradedBy</span><span class="sxs-lookup"><span data-stu-id="f8fb0-114">gradedBy</span></span>|[<span data-ttu-id="f8fb0-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="f8fb0-115">identitySet</span></span>](identityset.md)| <span data-ttu-id="f8fb0-116">Benutzer, der die Benotung haben.</span><span class="sxs-lookup"><span data-stu-id="f8fb0-116">User who did the grading.</span></span> |
|<span data-ttu-id="f8fb0-117">gradedDateTime</span><span class="sxs-lookup"><span data-stu-id="f8fb0-117">gradedDateTime</span></span>|<span data-ttu-id="f8fb0-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8fb0-118">DateTimeOffset</span></span>| <span data-ttu-id="f8fb0-119">Zeitpunkt Uhrzeit auf dieses Objekt zum Absenden die Klasse angewendet wurde.</span><span class="sxs-lookup"><span data-stu-id="f8fb0-119">Moment in time when the grade was applied to this submission object.</span></span> <span data-ttu-id="f8fb0-120">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="f8fb0-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f8fb0-121">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f8fb0-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f8fb0-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f8fb0-122">JSON representation</span></span>

<span data-ttu-id="f8fb0-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f8fb0-123">The following is a JSON representation of the resource.</span></span>

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