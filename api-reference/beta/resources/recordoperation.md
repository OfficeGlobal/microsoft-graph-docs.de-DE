---
title: Ressourcentyp recordOperation
description: Der RecordOperation-Typ
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 914b8d819fdbcc132d4e04cd12f5c0db9980f659
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577186"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="90c39-103">Ressourcentyp recordOperation</span><span class="sxs-lookup"><span data-stu-id="90c39-103">recordOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90c39-104">Der RecordOperation-Typ</span><span class="sxs-lookup"><span data-stu-id="90c39-104">The recordOperation type</span></span>

## <a name="properties"></a><span data-ttu-id="90c39-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="90c39-105">Properties</span></span>

| <span data-ttu-id="90c39-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="90c39-106">Property</span></span>                       | <span data-ttu-id="90c39-107">Typ</span><span class="sxs-lookup"><span data-stu-id="90c39-107">Type</span></span>                        | <span data-ttu-id="90c39-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="90c39-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="90c39-109">clientContext</span><span class="sxs-lookup"><span data-stu-id="90c39-109">clientContext</span></span>                  | <span data-ttu-id="90c39-110">String</span><span class="sxs-lookup"><span data-stu-id="90c39-110">String</span></span>                      | <span data-ttu-id="90c39-111">Der Clientkontext.</span><span class="sxs-lookup"><span data-stu-id="90c39-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="90c39-112">completionReason</span><span class="sxs-lookup"><span data-stu-id="90c39-112">completionReason</span></span>               | <span data-ttu-id="90c39-113">String</span><span class="sxs-lookup"><span data-stu-id="90c39-113">String</span></span>                      | <span data-ttu-id="90c39-114">Mögliche Werte: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="90c39-114">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="90c39-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="90c39-115">createdDateTime</span></span>                | <span data-ttu-id="90c39-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90c39-116">DateTimeOffset</span></span>              | <span data-ttu-id="90c39-117">Die Uhrzeit der Erstellung die Aufzeichnung.</span><span class="sxs-lookup"><span data-stu-id="90c39-117">The time when the recording was created.</span></span>                                                                                                          |
| <span data-ttu-id="90c39-118">id</span><span class="sxs-lookup"><span data-stu-id="90c39-118">id</span></span>                             | <span data-ttu-id="90c39-119">String</span><span class="sxs-lookup"><span data-stu-id="90c39-119">String</span></span>                      | <span data-ttu-id="90c39-120">Die Id des Server-Vorgang. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="90c39-120">The server operation id. Read-only.</span></span> <span data-ttu-id="90c39-121">Server generiert wurde.</span><span class="sxs-lookup"><span data-stu-id="90c39-121">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="90c39-122">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="90c39-122">lastActionDateTime</span></span>             | <span data-ttu-id="90c39-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90c39-123">DateTimeOffset</span></span>              | <span data-ttu-id="90c39-124">Der Zeitpunkt der letzten Aktion des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="90c39-124">The time of the last action of the operation.</span></span>                                                                                                     |
| <span data-ttu-id="90c39-125">recordResourceAccessToken</span><span class="sxs-lookup"><span data-stu-id="90c39-125">recordResourceAccessToken</span></span>      | <span data-ttu-id="90c39-126">String</span><span class="sxs-lookup"><span data-stu-id="90c39-126">String</span></span>                      | <span data-ttu-id="90c39-127">Das Zugriffstoken zum Abrufen der aufzeichnungs erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="90c39-127">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="90c39-128">recordResourceLocation</span><span class="sxs-lookup"><span data-stu-id="90c39-128">recordResourceLocation</span></span>         | <span data-ttu-id="90c39-129">String</span><span class="sxs-lookup"><span data-stu-id="90c39-129">String</span></span>                      | <span data-ttu-id="90c39-130">Der Speicherort, in dem die Aufzeichnung gespeichert ist.</span><span class="sxs-lookup"><span data-stu-id="90c39-130">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="90c39-131">resultInfo</span><span class="sxs-lookup"><span data-stu-id="90c39-131">resultInfo</span></span>                     | [<span data-ttu-id="90c39-132">resultInfo</span><span class="sxs-lookup"><span data-stu-id="90c39-132">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="90c39-133">Informationen zu den Ergebnissen.</span><span class="sxs-lookup"><span data-stu-id="90c39-133">The result information.</span></span>  <span data-ttu-id="90c39-134">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="90c39-134">Read-only.</span></span> <span data-ttu-id="90c39-135">Server generiert wurde.</span><span class="sxs-lookup"><span data-stu-id="90c39-135">Server generated.</span></span>                                                                                             |

## <a name="relationships"></a><span data-ttu-id="90c39-136">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="90c39-136">Relationships</span></span>
<span data-ttu-id="90c39-137">Keine</span><span class="sxs-lookup"><span data-stu-id="90c39-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="90c39-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="90c39-138">JSON representation</span></span>

<span data-ttu-id="90c39-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="90c39-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordOperation"
}-->
```json
{
  "clientContext": "String",
  "completionReason": "recordCompletionReason",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "recordResourceAccessToken": "String",
  "recordResourceLocation": "String",
  "resultInfo": {"@odata.type": "microsoft.graph.resultInfo"}
}
```

## <a name="example"></a><span data-ttu-id="90c39-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="90c39-140">Example</span></span>

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
