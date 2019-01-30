---
title: Ressourcentyp recordOperation
description: Der RecordOperation-Typ
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 6b9deb566e5b527a9f20db69441fa96908212a38
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641596"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="c6c7f-103">Ressourcentyp recordOperation</span><span class="sxs-lookup"><span data-stu-id="c6c7f-103">recordOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6c7f-104">Der RecordOperation-Typ</span><span class="sxs-lookup"><span data-stu-id="c6c7f-104">The recordOperation type</span></span>

## <a name="properties"></a><span data-ttu-id="c6c7f-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c6c7f-105">Properties</span></span>

| <span data-ttu-id="c6c7f-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c6c7f-106">Property</span></span>                       | <span data-ttu-id="c6c7f-107">Typ</span><span class="sxs-lookup"><span data-stu-id="c6c7f-107">Type</span></span>                        | <span data-ttu-id="c6c7f-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c6c7f-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c6c7f-109">clientContext</span><span class="sxs-lookup"><span data-stu-id="c6c7f-109">clientContext</span></span>                  | <span data-ttu-id="c6c7f-110">String</span><span class="sxs-lookup"><span data-stu-id="c6c7f-110">String</span></span>                      | <span data-ttu-id="c6c7f-111">Der Clientkontext.</span><span class="sxs-lookup"><span data-stu-id="c6c7f-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="c6c7f-112">completionReason</span><span class="sxs-lookup"><span data-stu-id="c6c7f-112">completionReason</span></span>               | <span data-ttu-id="c6c7f-113">String</span><span class="sxs-lookup"><span data-stu-id="c6c7f-113">String</span></span>                      | <span data-ttu-id="c6c7f-114">Mögliche Werte: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="c6c7f-114">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="c6c7f-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c6c7f-115">createdDateTime</span></span>                | <span data-ttu-id="c6c7f-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6c7f-116">DateTimeOffset</span></span>              | <span data-ttu-id="c6c7f-117">Die Uhrzeit der Erstellung die Aufzeichnung.</span><span class="sxs-lookup"><span data-stu-id="c6c7f-117">The time when the recording was created.</span></span>                                                                                                          |
| <span data-ttu-id="c6c7f-118">id</span><span class="sxs-lookup"><span data-stu-id="c6c7f-118">id</span></span>                             | <span data-ttu-id="c6c7f-119">String</span><span class="sxs-lookup"><span data-stu-id="c6c7f-119">String</span></span>                      | <span data-ttu-id="c6c7f-120">Die Id des Server-Vorgang. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c6c7f-120">The server operation id. Read-only.</span></span> <span data-ttu-id="c6c7f-121">Vom Server generiert.</span><span class="sxs-lookup"><span data-stu-id="c6c7f-121">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="c6c7f-122">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="c6c7f-122">lastActionDateTime</span></span>             | <span data-ttu-id="c6c7f-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6c7f-123">DateTimeOffset</span></span>              | <span data-ttu-id="c6c7f-124">Der Zeitpunkt der letzten Aktion des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="c6c7f-124">The time of the last action of the operation.</span></span>                                                                                                     |
| <span data-ttu-id="c6c7f-125">recordResourceAccessToken</span><span class="sxs-lookup"><span data-stu-id="c6c7f-125">recordResourceAccessToken</span></span>      | <span data-ttu-id="c6c7f-126">String</span><span class="sxs-lookup"><span data-stu-id="c6c7f-126">String</span></span>                      | <span data-ttu-id="c6c7f-127">Das Zugriffstoken zum Abrufen der aufzeichnungs erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c6c7f-127">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="c6c7f-128">recordResourceLocation</span><span class="sxs-lookup"><span data-stu-id="c6c7f-128">recordResourceLocation</span></span>         | <span data-ttu-id="c6c7f-129">String</span><span class="sxs-lookup"><span data-stu-id="c6c7f-129">String</span></span>                      | <span data-ttu-id="c6c7f-130">Der Speicherort, in dem die Aufzeichnung gespeichert ist.</span><span class="sxs-lookup"><span data-stu-id="c6c7f-130">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="c6c7f-131">resultInfo</span><span class="sxs-lookup"><span data-stu-id="c6c7f-131">resultInfo</span></span>                     | [<span data-ttu-id="c6c7f-132">resultInfo</span><span class="sxs-lookup"><span data-stu-id="c6c7f-132">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="c6c7f-133">Die Ergebnisinformationen.</span><span class="sxs-lookup"><span data-stu-id="c6c7f-133">The result information.</span></span>  <span data-ttu-id="c6c7f-134">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c6c7f-134">Read-only.</span></span> <span data-ttu-id="c6c7f-135">Vom Server generiert.</span><span class="sxs-lookup"><span data-stu-id="c6c7f-135">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="c6c7f-136">status</span><span class="sxs-lookup"><span data-stu-id="c6c7f-136">status</span></span>                         | <span data-ttu-id="c6c7f-137">String</span><span class="sxs-lookup"><span data-stu-id="c6c7f-137">String</span></span>                      | <span data-ttu-id="c6c7f-138">Mögliche Werte: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="c6c7f-138">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="c6c7f-139">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c6c7f-139">Read-only.</span></span> <span data-ttu-id="c6c7f-140">Vom Server generiert.</span><span class="sxs-lookup"><span data-stu-id="c6c7f-140">Server generated.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="c6c7f-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c6c7f-141">Relationships</span></span>
<span data-ttu-id="c6c7f-142">Keine</span><span class="sxs-lookup"><span data-stu-id="c6c7f-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c6c7f-143">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c6c7f-143">JSON representation</span></span>

<span data-ttu-id="c6c7f-144">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c6c7f-144">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="c6c7f-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c6c7f-145">Example</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "recordOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/recordoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
