---
title: Ressourcentyp recordOperation
description: Der RecordOperation-Typ
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: be6a124fcd7175489679a8c2392218530d510e9e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880017"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="e5fe3-103">Ressourcentyp recordOperation</span><span class="sxs-lookup"><span data-stu-id="e5fe3-103">recordOperation resource type</span></span>

> <span data-ttu-id="e5fe3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e5fe3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5fe3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e5fe3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e5fe3-106">Der RecordOperation-Typ</span><span class="sxs-lookup"><span data-stu-id="e5fe3-106">The recordOperation type</span></span>

## <a name="properties"></a><span data-ttu-id="e5fe3-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e5fe3-107">Properties</span></span>

| <span data-ttu-id="e5fe3-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e5fe3-108">Property</span></span>                       | <span data-ttu-id="e5fe3-109">Typ</span><span class="sxs-lookup"><span data-stu-id="e5fe3-109">Type</span></span>                        | <span data-ttu-id="e5fe3-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e5fe3-110">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e5fe3-111">clientContext</span><span class="sxs-lookup"><span data-stu-id="e5fe3-111">clientContext</span></span>                  | <span data-ttu-id="e5fe3-112">String</span><span class="sxs-lookup"><span data-stu-id="e5fe3-112">String</span></span>                      | <span data-ttu-id="e5fe3-113">Der Clientkontext.</span><span class="sxs-lookup"><span data-stu-id="e5fe3-113">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="e5fe3-114">completionReason</span><span class="sxs-lookup"><span data-stu-id="e5fe3-114">completionReason</span></span>               | <span data-ttu-id="e5fe3-115">String</span><span class="sxs-lookup"><span data-stu-id="e5fe3-115">String</span></span>                      | <span data-ttu-id="e5fe3-116">Mögliche Werte: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="e5fe3-116">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="e5fe3-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e5fe3-117">createdDateTime</span></span>                | <span data-ttu-id="e5fe3-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5fe3-118">DateTimeOffset</span></span>              | <span data-ttu-id="e5fe3-119">Die Uhrzeit der Erstellung die Aufzeichnung.</span><span class="sxs-lookup"><span data-stu-id="e5fe3-119">The time when the recording was created.</span></span>                                                                                                          |
| <span data-ttu-id="e5fe3-120">id</span><span class="sxs-lookup"><span data-stu-id="e5fe3-120">id</span></span>                             | <span data-ttu-id="e5fe3-121">String</span><span class="sxs-lookup"><span data-stu-id="e5fe3-121">String</span></span>                      | <span data-ttu-id="e5fe3-122">Die Id des Server-Vorgang. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e5fe3-122">The server operation id. Read-only.</span></span> <span data-ttu-id="e5fe3-123">Server generiert wurde.</span><span class="sxs-lookup"><span data-stu-id="e5fe3-123">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="e5fe3-124">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="e5fe3-124">lastActionDateTime</span></span>             | <span data-ttu-id="e5fe3-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5fe3-125">DateTimeOffset</span></span>              | <span data-ttu-id="e5fe3-126">Der Zeitpunkt der letzten Aktion des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="e5fe3-126">The time of the last action of the operation.</span></span>                                                                                                     |
| <span data-ttu-id="e5fe3-127">recordResourceAccessToken</span><span class="sxs-lookup"><span data-stu-id="e5fe3-127">recordResourceAccessToken</span></span>      | <span data-ttu-id="e5fe3-128">String</span><span class="sxs-lookup"><span data-stu-id="e5fe3-128">String</span></span>                      | <span data-ttu-id="e5fe3-129">Das Zugriffstoken zum Abrufen der aufzeichnungs erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e5fe3-129">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="e5fe3-130">recordResourceLocation</span><span class="sxs-lookup"><span data-stu-id="e5fe3-130">recordResourceLocation</span></span>         | <span data-ttu-id="e5fe3-131">String</span><span class="sxs-lookup"><span data-stu-id="e5fe3-131">String</span></span>                      | <span data-ttu-id="e5fe3-132">Der Speicherort, in dem die Aufzeichnung gespeichert ist.</span><span class="sxs-lookup"><span data-stu-id="e5fe3-132">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="e5fe3-133">resultInfo</span><span class="sxs-lookup"><span data-stu-id="e5fe3-133">resultInfo</span></span>                     | [<span data-ttu-id="e5fe3-134">resultInfo</span><span class="sxs-lookup"><span data-stu-id="e5fe3-134">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="e5fe3-135">Informationen zu den Ergebnissen.</span><span class="sxs-lookup"><span data-stu-id="e5fe3-135">The result information.</span></span>  <span data-ttu-id="e5fe3-136">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e5fe3-136">Read-only.</span></span> <span data-ttu-id="e5fe3-137">Server generiert wurde.</span><span class="sxs-lookup"><span data-stu-id="e5fe3-137">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="e5fe3-138">status</span><span class="sxs-lookup"><span data-stu-id="e5fe3-138">status</span></span>                         | <span data-ttu-id="e5fe3-139">String</span><span class="sxs-lookup"><span data-stu-id="e5fe3-139">String</span></span>                      | <span data-ttu-id="e5fe3-140">Mögliche Werte: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="e5fe3-140">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="e5fe3-141">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e5fe3-141">Read-only.</span></span> <span data-ttu-id="e5fe3-142">Server generiert wurde.</span><span class="sxs-lookup"><span data-stu-id="e5fe3-142">Server generated.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="e5fe3-143">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e5fe3-143">Relationships</span></span>
<span data-ttu-id="e5fe3-144">Keine</span><span class="sxs-lookup"><span data-stu-id="e5fe3-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5fe3-145">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e5fe3-145">JSON representation</span></span>

<span data-ttu-id="e5fe3-146">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e5fe3-146">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordOperation"
}-->
```json
{
  "clientContext": "String",
  "completionReason": "operationCanceled | stopToneDetected | maxRecordDurationReached | initialSilenceTimeout | maxSilenceTimeout | playPromptFailed | playBeepFailed | mediaReceiveTimeout | unspecifiedError | none",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "recordResourceAccessToken": "String",
  "recordResourceLocation": "String",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a><span data-ttu-id="e5fe3-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e5fe3-147">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.recordOperation",
  "truncated": true
}-->
```json
{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "recordResourceAccessToken": "<access-token>",
  "recordResourceLocation": "https://resource.location/ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "status": "completed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recordOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
