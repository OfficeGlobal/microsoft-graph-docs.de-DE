---
title: Ressourcentyp recordingInfo
description: Aufzeichnung von Informationen für einen Teilnehmer.
author: VinodRavichandran
ms.openlocfilehash: 709edcc6d473ce610cbba7f628e4ebc5057b779c
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380303"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="b2911-103">Ressourcentyp recordingInfo</span><span class="sxs-lookup"><span data-stu-id="b2911-103">recordingInfo resource type</span></span>

> <span data-ttu-id="b2911-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b2911-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2911-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b2911-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b2911-106">Aufzeichnung von Informationen für einen Teilnehmer.</span><span class="sxs-lookup"><span data-stu-id="b2911-106">Recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="b2911-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b2911-107">Properties</span></span>

| <span data-ttu-id="b2911-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b2911-108">Property</span></span>       | <span data-ttu-id="b2911-109">Typ</span><span class="sxs-lookup"><span data-stu-id="b2911-109">Type</span></span>    | <span data-ttu-id="b2911-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b2911-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b2911-111">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="b2911-111">initiatedBy</span></span> | [<span data-ttu-id="b2911-112">participantInfo</span><span class="sxs-lookup"><span data-stu-id="b2911-112">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="b2911-113">Der Teilnehmer, der die Aufzeichnung initiiert hat.</span><span class="sxs-lookup"><span data-stu-id="b2911-113">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="b2911-114">status</span><span class="sxs-lookup"><span data-stu-id="b2911-114">status</span></span> | <span data-ttu-id="b2911-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b2911-115">String</span></span> | <span data-ttu-id="b2911-116">Mögliche Werte sind: `recordingCapable`, `notRecording` und `startedRecording`.</span><span class="sxs-lookup"><span data-stu-id="b2911-116">Possible values are: `recordingCapable`, `notRecording`, `startedRecording`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b2911-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b2911-117">JSON representation</span></span>

<span data-ttu-id="b2911-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b2911-118">The following is a JSON representation of the resource.</span></span>

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
