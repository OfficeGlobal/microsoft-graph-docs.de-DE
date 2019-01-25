---
title: Ressourcentyp recordingInfo
description: Aufzeichnung von Informationen für einen Teilnehmer.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 6025259bafdcff78c3c7dbfa19aa39f5f6648f84
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525675"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="03bf2-103">Ressourcentyp recordingInfo</span><span class="sxs-lookup"><span data-stu-id="03bf2-103">recordingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03bf2-104">Aufzeichnung von Informationen für einen Teilnehmer.</span><span class="sxs-lookup"><span data-stu-id="03bf2-104">Recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="03bf2-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="03bf2-105">Properties</span></span>

| <span data-ttu-id="03bf2-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="03bf2-106">Property</span></span>       | <span data-ttu-id="03bf2-107">Typ</span><span class="sxs-lookup"><span data-stu-id="03bf2-107">Type</span></span>    | <span data-ttu-id="03bf2-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="03bf2-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="03bf2-109">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="03bf2-109">initiatedBy</span></span> | [<span data-ttu-id="03bf2-110">participantInfo</span><span class="sxs-lookup"><span data-stu-id="03bf2-110">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="03bf2-111">Der Teilnehmer, der die Aufzeichnung initiiert hat.</span><span class="sxs-lookup"><span data-stu-id="03bf2-111">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="03bf2-112">status</span><span class="sxs-lookup"><span data-stu-id="03bf2-112">status</span></span> | <span data-ttu-id="03bf2-113">String</span><span class="sxs-lookup"><span data-stu-id="03bf2-113">String</span></span> | <span data-ttu-id="03bf2-114">Mögliche Werte sind: `recordingCapable`, `notRecording` und `startedRecording`.</span><span class="sxs-lookup"><span data-stu-id="03bf2-114">Possible values are: `recordingCapable`, `notRecording`, `startedRecording`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="03bf2-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="03bf2-115">JSON representation</span></span>

<span data-ttu-id="03bf2-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="03bf2-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordingInfo"
}-->
```json
{
  "initiatedBy": {"@odata.type": "#microsoft.graph.participantInfo"},
  "status": "recordingCapable | notRecording | startedRecording"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recordingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/recordinginfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
