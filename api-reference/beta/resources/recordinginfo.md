---
title: Ressourcentyp recordingInfo
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 92af3fcb52ab08f3f25a2c16cc720a4053a9bdfa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061464"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="fe963-103">Ressourcentyp recordingInfo</span><span class="sxs-lookup"><span data-stu-id="fe963-103">recordingInfo resource type</span></span>

> <span data-ttu-id="fe963-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fe963-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe963-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fe963-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="fe963-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fe963-106">Properties</span></span>

| <span data-ttu-id="fe963-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fe963-107">Property</span></span>       | <span data-ttu-id="fe963-108">Typ</span><span class="sxs-lookup"><span data-stu-id="fe963-108">Type</span></span>    | <span data-ttu-id="fe963-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fe963-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fe963-110">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="fe963-110">initiatedBy</span></span> | [<span data-ttu-id="fe963-111">participantInfo</span><span class="sxs-lookup"><span data-stu-id="fe963-111">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="fe963-112">Der Teilnehmer, der die Aufzeichnung initiiert hat.</span><span class="sxs-lookup"><span data-stu-id="fe963-112">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="fe963-113">status</span><span class="sxs-lookup"><span data-stu-id="fe963-113">status</span></span> | <span data-ttu-id="fe963-114">String</span><span class="sxs-lookup"><span data-stu-id="fe963-114">String</span></span> | <span data-ttu-id="fe963-115">Mögliche Werte sind: `recordingCapable`, `notRecording` und `startedRecording`.</span><span class="sxs-lookup"><span data-stu-id="fe963-115">Possible values are: `recordingCapable`, `notRecording`, `startedRecording`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fe963-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fe963-116">JSON representation</span></span>

<span data-ttu-id="fe963-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fe963-117">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "recordingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
