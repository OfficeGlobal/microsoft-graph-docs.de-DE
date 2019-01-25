---
title: Ressourcentyp playPromptOperation
description: Abrufen des Ergebnisses der Aktion PlayPrompt PlayPrompt-Vorgang.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a6ecdb06c910923d35f9d36590ad09fd7835fccb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515202"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="e575d-103">Ressourcentyp playPromptOperation</span><span class="sxs-lookup"><span data-stu-id="e575d-103">playPromptOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e575d-104">Abrufen des Ergebnisses der Aktion PlayPrompt PlayPrompt-Vorgang.</span><span class="sxs-lookup"><span data-stu-id="e575d-104">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="e575d-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e575d-105">Properties</span></span>

| <span data-ttu-id="e575d-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e575d-106">Property</span></span>            | <span data-ttu-id="e575d-107">Typ</span><span class="sxs-lookup"><span data-stu-id="e575d-107">Type</span></span>                        | <span data-ttu-id="e575d-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e575d-108">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="e575d-109">ClientContext</span><span class="sxs-lookup"><span data-stu-id="e575d-109">clientContext</span></span>       | <span data-ttu-id="e575d-110">String</span><span class="sxs-lookup"><span data-stu-id="e575d-110">String</span></span>                      | <span data-ttu-id="e575d-111">Der Clientkontext.</span><span class="sxs-lookup"><span data-stu-id="e575d-111">The client context.</span></span>                                                                |
| <span data-ttu-id="e575d-112">completionReason</span><span class="sxs-lookup"><span data-stu-id="e575d-112">completionReason</span></span>    | <span data-ttu-id="e575d-113">String</span><span class="sxs-lookup"><span data-stu-id="e575d-113">String</span></span>                      | <span data-ttu-id="e575d-114">Mögliche Werte sind: `unknown`, `completedSuccessfully` und `mediaOperationCanceled`.</span><span class="sxs-lookup"><span data-stu-id="e575d-114">Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span></span> |
| <span data-ttu-id="e575d-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e575d-115">createdDateTime</span></span>     | <span data-ttu-id="e575d-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e575d-116">DateTimeOffset</span></span>              | <span data-ttu-id="e575d-117">Die Startzeit des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="e575d-117">The start time of the operation.</span></span>                                                   |
| <span data-ttu-id="e575d-118">id</span><span class="sxs-lookup"><span data-stu-id="e575d-118">id</span></span>                  | <span data-ttu-id="e575d-119">String</span><span class="sxs-lookup"><span data-stu-id="e575d-119">String</span></span>                      | <span data-ttu-id="e575d-120">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e575d-120">Read-only.</span></span>                                                                         |
| <span data-ttu-id="e575d-121">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="e575d-121">lastActionDateTime</span></span>  | <span data-ttu-id="e575d-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e575d-122">DateTimeOffset</span></span>              | <span data-ttu-id="e575d-123">Der Zeitpunkt der letzten Aktion des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="e575d-123">The time of the last action of the operation.</span></span>                                      |
| <span data-ttu-id="e575d-124">resultInfo</span><span class="sxs-lookup"><span data-stu-id="e575d-124">resultInfo</span></span>          | [<span data-ttu-id="e575d-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="e575d-125">resultInfo</span></span>](resultInfo.md) | <span data-ttu-id="e575d-126">Informationen zu den Ergebnissen.</span><span class="sxs-lookup"><span data-stu-id="e575d-126">The result information.</span></span> <span data-ttu-id="e575d-127">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e575d-127">Read-only.</span></span> <span data-ttu-id="e575d-128">Server generiert wurde.</span><span class="sxs-lookup"><span data-stu-id="e575d-128">Server generated.</span></span>                               |
| <span data-ttu-id="e575d-129">status</span><span class="sxs-lookup"><span data-stu-id="e575d-129">status</span></span>              | <span data-ttu-id="e575d-130">String</span><span class="sxs-lookup"><span data-stu-id="e575d-130">String</span></span>                      | <span data-ttu-id="e575d-131">Mögliche Werte: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="e575d-131">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="e575d-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e575d-132">Relationships</span></span>
<span data-ttu-id="e575d-133">Keine</span><span class="sxs-lookup"><span data-stu-id="e575d-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e575d-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e575d-134">JSON representation</span></span>

<span data-ttu-id="e575d-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e575d-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.playPromptOperation"
}-->
```json
{
  "clientContext": "String",
  "completionReason": "unknown | completedSuccessfully | mediaOperationCanceled",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "playPromptOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/playpromptoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
