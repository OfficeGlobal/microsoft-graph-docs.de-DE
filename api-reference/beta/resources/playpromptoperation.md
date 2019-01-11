---
title: Ressourcentyp playPromptOperation
description: Abrufen des Ergebnisses der Aktion PlayPrompt PlayPrompt-Vorgang.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: bc18b8f64dedd3fa4d758778bbee37c6bcfd46c6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814378"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="fec12-103">Ressourcentyp playPromptOperation</span><span class="sxs-lookup"><span data-stu-id="fec12-103">playPromptOperation resource type</span></span>

> <span data-ttu-id="fec12-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fec12-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fec12-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fec12-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fec12-106">Abrufen des Ergebnisses der Aktion PlayPrompt PlayPrompt-Vorgang.</span><span class="sxs-lookup"><span data-stu-id="fec12-106">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="fec12-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fec12-107">Properties</span></span>

| <span data-ttu-id="fec12-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fec12-108">Property</span></span>            | <span data-ttu-id="fec12-109">Typ</span><span class="sxs-lookup"><span data-stu-id="fec12-109">Type</span></span>                        | <span data-ttu-id="fec12-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fec12-110">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="fec12-111">clientContext</span><span class="sxs-lookup"><span data-stu-id="fec12-111">clientContext</span></span>       | <span data-ttu-id="fec12-112">String</span><span class="sxs-lookup"><span data-stu-id="fec12-112">String</span></span>                      | <span data-ttu-id="fec12-113">Der Clientkontext.</span><span class="sxs-lookup"><span data-stu-id="fec12-113">The client context.</span></span>                                                                |
| <span data-ttu-id="fec12-114">completionReason</span><span class="sxs-lookup"><span data-stu-id="fec12-114">completionReason</span></span>    | <span data-ttu-id="fec12-115">String</span><span class="sxs-lookup"><span data-stu-id="fec12-115">String</span></span>                      | <span data-ttu-id="fec12-116">Mögliche Werte sind: `unknown`, `completedSuccessfully` und `mediaOperationCanceled`.</span><span class="sxs-lookup"><span data-stu-id="fec12-116">Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span></span> |
| <span data-ttu-id="fec12-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fec12-117">createdDateTime</span></span>     | <span data-ttu-id="fec12-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fec12-118">DateTimeOffset</span></span>              | <span data-ttu-id="fec12-119">Die Startzeit des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="fec12-119">The start time of the operation.</span></span>                                                   |
| <span data-ttu-id="fec12-120">id</span><span class="sxs-lookup"><span data-stu-id="fec12-120">id</span></span>                  | <span data-ttu-id="fec12-121">String</span><span class="sxs-lookup"><span data-stu-id="fec12-121">String</span></span>                      | <span data-ttu-id="fec12-122">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fec12-122">Read-only.</span></span>                                                                         |
| <span data-ttu-id="fec12-123">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="fec12-123">lastActionDateTime</span></span>  | <span data-ttu-id="fec12-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fec12-124">DateTimeOffset</span></span>              | <span data-ttu-id="fec12-125">Der Zeitpunkt der letzten Aktion des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="fec12-125">The time of the last action of the operation.</span></span>                                      |
| <span data-ttu-id="fec12-126">resultInfo</span><span class="sxs-lookup"><span data-stu-id="fec12-126">resultInfo</span></span>          | [<span data-ttu-id="fec12-127">resultInfo</span><span class="sxs-lookup"><span data-stu-id="fec12-127">resultInfo</span></span>](resultInfo.md) | <span data-ttu-id="fec12-128">Informationen zu den Ergebnissen.</span><span class="sxs-lookup"><span data-stu-id="fec12-128">The result information.</span></span> <span data-ttu-id="fec12-129">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fec12-129">Read-only.</span></span> <span data-ttu-id="fec12-130">Server generiert wurde.</span><span class="sxs-lookup"><span data-stu-id="fec12-130">Server generated.</span></span>                               |
| <span data-ttu-id="fec12-131">status</span><span class="sxs-lookup"><span data-stu-id="fec12-131">status</span></span>              | <span data-ttu-id="fec12-132">String</span><span class="sxs-lookup"><span data-stu-id="fec12-132">String</span></span>                      | <span data-ttu-id="fec12-133">Mögliche Werte: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="fec12-133">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="fec12-134">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fec12-134">Relationships</span></span>
<span data-ttu-id="fec12-135">Keine</span><span class="sxs-lookup"><span data-stu-id="fec12-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fec12-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fec12-136">JSON representation</span></span>

<span data-ttu-id="fec12-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fec12-137">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "playPromptOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
