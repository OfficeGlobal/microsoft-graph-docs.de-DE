---
title: Ressourcentyp educationFeedback
description: Bewertung von Lehrer an einen Schüler. Diese Eigenschaft stellt sowohl den Text in das Feedback zusammen mit der, die an.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 90e55b20b371d04bc3c6d45bb84fe6bf42157a2f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515636"
---
# <a name="educationfeedback-resource-type"></a><span data-ttu-id="36ab1-104">Ressourcentyp educationFeedback</span><span class="sxs-lookup"><span data-stu-id="36ab1-104">educationFeedback resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36ab1-105">Bewertung von Lehrer an einen Schüler.</span><span class="sxs-lookup"><span data-stu-id="36ab1-105">Feedback from a teacher to a student.</span></span> <span data-ttu-id="36ab1-106">Diese Eigenschaft stellt sowohl den Text in das Feedback zusammen mit der, die an.</span><span class="sxs-lookup"><span data-stu-id="36ab1-106">This property represents both the text part of the feedback along with the who.</span></span>


## <a name="properties"></a><span data-ttu-id="36ab1-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="36ab1-107">Properties</span></span>
| <span data-ttu-id="36ab1-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="36ab1-108">Property</span></span>     | <span data-ttu-id="36ab1-109">Typ</span><span class="sxs-lookup"><span data-stu-id="36ab1-109">Type</span></span>   |<span data-ttu-id="36ab1-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="36ab1-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36ab1-111">feedbackBy</span><span class="sxs-lookup"><span data-stu-id="36ab1-111">feedbackBy</span></span>|[<span data-ttu-id="36ab1-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="36ab1-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="36ab1-113">Benutzer, die das Feedback erstellt hat.</span><span class="sxs-lookup"><span data-stu-id="36ab1-113">User who created the feedback.</span></span>|
|<span data-ttu-id="36ab1-114">feedbackDateTime</span><span class="sxs-lookup"><span data-stu-id="36ab1-114">feedbackDateTime</span></span>|<span data-ttu-id="36ab1-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36ab1-115">DateTimeOffset</span></span>|<span data-ttu-id="36ab1-116">Wenn das Feedback weitergegebenen Zeitpunkt.</span><span class="sxs-lookup"><span data-stu-id="36ab1-116">Moment in time when the feedback was given.</span></span> <span data-ttu-id="36ab1-117">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="36ab1-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="36ab1-118">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="36ab1-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="36ab1-119">text</span><span class="sxs-lookup"><span data-stu-id="36ab1-119">text</span></span>|[<span data-ttu-id="36ab1-120">itemBody</span><span class="sxs-lookup"><span data-stu-id="36ab1-120">itemBody</span></span>](itembody.md)|<span data-ttu-id="36ab1-121">Feedback</span><span class="sxs-lookup"><span data-stu-id="36ab1-121">Feedback.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="36ab1-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="36ab1-122">JSON representation</span></span>

<span data-ttu-id="36ab1-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="36ab1-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFeedback"
}-->

```json
{
  "feedbackBy": {"@odata.type": "microsoft.graph.identitySet"},
  "feedbackDateTime": "String (timestamp)",
  "text": {"@odata.type": "microsoft.graph.itemBody"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationFeedback resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationfeedback.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
