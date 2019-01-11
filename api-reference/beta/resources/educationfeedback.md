---
title: Ressourcentyp educationFeedback
description: Bewertung von Lehrer an einen Schüler. Diese Eigenschaft stellt sowohl den Text in das Feedback zusammen mit der, die an.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 0d08f3bc5c7b4882693cdcbba41b364734c6ccef
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873563"
---
# <a name="educationfeedback-resource-type"></a><span data-ttu-id="6bc96-104">Ressourcentyp educationFeedback</span><span class="sxs-lookup"><span data-stu-id="6bc96-104">educationFeedback resource type</span></span>

> <span data-ttu-id="6bc96-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6bc96-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6bc96-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6bc96-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6bc96-107">Bewertung von Lehrer an einen Schüler.</span><span class="sxs-lookup"><span data-stu-id="6bc96-107">Feedback from a teacher to a student.</span></span> <span data-ttu-id="6bc96-108">Diese Eigenschaft stellt sowohl den Text in das Feedback zusammen mit der, die an.</span><span class="sxs-lookup"><span data-stu-id="6bc96-108">This property represents both the text part of the feedback along with the who.</span></span>


## <a name="properties"></a><span data-ttu-id="6bc96-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6bc96-109">Properties</span></span>
| <span data-ttu-id="6bc96-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6bc96-110">Property</span></span>     | <span data-ttu-id="6bc96-111">Typ</span><span class="sxs-lookup"><span data-stu-id="6bc96-111">Type</span></span>   |<span data-ttu-id="6bc96-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6bc96-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6bc96-113">feedbackBy</span><span class="sxs-lookup"><span data-stu-id="6bc96-113">feedbackBy</span></span>|[<span data-ttu-id="6bc96-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="6bc96-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="6bc96-115">Benutzer, die das Feedback erstellt hat.</span><span class="sxs-lookup"><span data-stu-id="6bc96-115">User who created the feedback.</span></span>|
|<span data-ttu-id="6bc96-116">feedbackDateTime</span><span class="sxs-lookup"><span data-stu-id="6bc96-116">feedbackDateTime</span></span>|<span data-ttu-id="6bc96-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bc96-117">DateTimeOffset</span></span>|<span data-ttu-id="6bc96-118">Wenn das Feedback weitergegebenen Zeitpunkt.</span><span class="sxs-lookup"><span data-stu-id="6bc96-118">Moment in time when the feedback was given.</span></span> <span data-ttu-id="6bc96-119">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="6bc96-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6bc96-120">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="6bc96-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6bc96-121">text</span><span class="sxs-lookup"><span data-stu-id="6bc96-121">text</span></span>|[<span data-ttu-id="6bc96-122">itemBody</span><span class="sxs-lookup"><span data-stu-id="6bc96-122">itemBody</span></span>](itembody.md)|<span data-ttu-id="6bc96-123">Feedback.</span><span class="sxs-lookup"><span data-stu-id="6bc96-123">Feedback.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6bc96-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6bc96-124">JSON representation</span></span>

<span data-ttu-id="6bc96-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6bc96-125">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationFeedback resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
