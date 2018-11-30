---
title: Ressourcentyp recordOperation
description: Der RecordOperation-Typ
ms.openlocfilehash: 5863e5ef84b00c65cd0806af8a3364fe3d1ab73f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059494"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="c90ec-103">Ressourcentyp recordOperation</span><span class="sxs-lookup"><span data-stu-id="c90ec-103">recordOperation resource type</span></span>

> <span data-ttu-id="c90ec-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c90ec-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c90ec-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c90ec-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c90ec-106">Der RecordOperation-Typ</span><span class="sxs-lookup"><span data-stu-id="c90ec-106">The recordOperation type</span></span>

## <a name="properties"></a><span data-ttu-id="c90ec-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c90ec-107">Properties</span></span>

| <span data-ttu-id="c90ec-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c90ec-108">Property</span></span>                       | <span data-ttu-id="c90ec-109">Typ</span><span class="sxs-lookup"><span data-stu-id="c90ec-109">Type</span></span>                        | <span data-ttu-id="c90ec-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c90ec-110">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c90ec-111">clientContext</span><span class="sxs-lookup"><span data-stu-id="c90ec-111">clientContext</span></span>                  | <span data-ttu-id="c90ec-112">String</span><span class="sxs-lookup"><span data-stu-id="c90ec-112">String</span></span>                      | <span data-ttu-id="c90ec-113">Der Clientkontext.</span><span class="sxs-lookup"><span data-stu-id="c90ec-113">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="c90ec-114">completionReason</span><span class="sxs-lookup"><span data-stu-id="c90ec-114">completionReason</span></span>               | <span data-ttu-id="c90ec-115">String</span><span class="sxs-lookup"><span data-stu-id="c90ec-115">String</span></span>                      | <span data-ttu-id="c90ec-116">Mögliche Werte: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`.</span><span class="sxs-lookup"><span data-stu-id="c90ec-116">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`.</span></span> |
| <span data-ttu-id="c90ec-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c90ec-117">createdDateTime</span></span>                | <span data-ttu-id="c90ec-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c90ec-118">DateTimeOffset</span></span>              | <span data-ttu-id="c90ec-119">Die Uhrzeit der Erstellung die Aufzeichnung.</span><span class="sxs-lookup"><span data-stu-id="c90ec-119">The time when the recording was created.</span></span>                                                                                                          |
| <span data-ttu-id="c90ec-120">id</span><span class="sxs-lookup"><span data-stu-id="c90ec-120">id</span></span>                             | <span data-ttu-id="c90ec-121">String</span><span class="sxs-lookup"><span data-stu-id="c90ec-121">String</span></span>                      | <span data-ttu-id="c90ec-122">Die Id des Server-Vorgang. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c90ec-122">The server operation id. Read-only.</span></span> <span data-ttu-id="c90ec-123">Server generiert wurde.</span><span class="sxs-lookup"><span data-stu-id="c90ec-123">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="c90ec-124">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="c90ec-124">lastActionDateTime</span></span>             | <span data-ttu-id="c90ec-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c90ec-125">DateTimeOffset</span></span>              | <span data-ttu-id="c90ec-126">Der Zeitpunkt der letzten Aktion des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="c90ec-126">The time of the last action of the operation.</span></span>                                                                                                     |
| <span data-ttu-id="c90ec-127">recordResourceLocation</span><span class="sxs-lookup"><span data-stu-id="c90ec-127">recordResourceLocation</span></span>         | <span data-ttu-id="c90ec-128">String</span><span class="sxs-lookup"><span data-stu-id="c90ec-128">String</span></span>                      | <span data-ttu-id="c90ec-129">Der Speicherort, in dem die Aufzeichnung gespeichert ist.</span><span class="sxs-lookup"><span data-stu-id="c90ec-129">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="c90ec-130">recordResourceAccessToken</span><span class="sxs-lookup"><span data-stu-id="c90ec-130">recordResourceAccessToken</span></span>      | <span data-ttu-id="c90ec-131">String</span><span class="sxs-lookup"><span data-stu-id="c90ec-131">String</span></span>                      | <span data-ttu-id="c90ec-132">Das Zugriffstoken zum Abrufen der aufzeichnungs erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c90ec-132">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="c90ec-133">resultInfo</span><span class="sxs-lookup"><span data-stu-id="c90ec-133">resultInfo</span></span>                     | [<span data-ttu-id="c90ec-134">resultInfo</span><span class="sxs-lookup"><span data-stu-id="c90ec-134">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="c90ec-135">Informationen zu den Ergebnissen.</span><span class="sxs-lookup"><span data-stu-id="c90ec-135">The result information.</span></span>  <span data-ttu-id="c90ec-136">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c90ec-136">Read-only.</span></span> <span data-ttu-id="c90ec-137">Server generiert wurde.</span><span class="sxs-lookup"><span data-stu-id="c90ec-137">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="c90ec-138">status</span><span class="sxs-lookup"><span data-stu-id="c90ec-138">status</span></span>                         | <span data-ttu-id="c90ec-139">String</span><span class="sxs-lookup"><span data-stu-id="c90ec-139">String</span></span>                      | <span data-ttu-id="c90ec-140">Mögliche Werte: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="c90ec-140">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="c90ec-141">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c90ec-141">Read-only.</span></span> <span data-ttu-id="c90ec-142">Server generiert wurde.</span><span class="sxs-lookup"><span data-stu-id="c90ec-142">Server generated.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="c90ec-143">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c90ec-143">Relationships</span></span>
<span data-ttu-id="c90ec-144">Keine</span><span class="sxs-lookup"><span data-stu-id="c90ec-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c90ec-145">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c90ec-145">JSON representation</span></span>

<span data-ttu-id="c90ec-146">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c90ec-146">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordOperation"
}-->
```json
{
  "clientContext": "String",
  "completionReason": "operationCanceled | stopToneDetected | maxRecordDurationReached | initialSilenceTimeout | maxSilenceTimeout | playPromptFailed | playBeepFailed | mediaReceiveTimeout | unspecifiedError",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "recordResourceLocation": "String",
  "recordResourceAccessToken": "String",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a><span data-ttu-id="c90ec-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c90ec-147">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.recordOperation",
  "truncated": true
}-->
```json
{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "recordResourceLocation": "https://resource.location/ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "recordResourceAccessToken": "<access-token>",
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
