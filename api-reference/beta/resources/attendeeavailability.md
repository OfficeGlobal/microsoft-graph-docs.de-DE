---
title: Ressourcentyp „attendeeAvailability“
description: Typ und Verfügbarkeit eines Teilnehmers
ms.openlocfilehash: ddea2be21f2dd9290637536e2a428e25fc03fcca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058468"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="ce6e8-103">Ressourcentyp „attendeeAvailability“</span><span class="sxs-lookup"><span data-stu-id="ce6e8-103">attendeeAvailability resource type</span></span>

> <span data-ttu-id="ce6e8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ce6e8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ce6e8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ce6e8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ce6e8-106">Typ und Verfügbarkeit eines Teilnehmers</span><span class="sxs-lookup"><span data-stu-id="ce6e8-106">The type and availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce6e8-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ce6e8-107">JSON representation</span></span>

<span data-ttu-id="ce6e8-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ce6e8-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeAvailability"
}-->

```json
{
  "attendee": {"@odata.type": "microsoft.graph.attendeeBase"},
  "availability": "String"
}

```
## <a name="properties"></a><span data-ttu-id="ce6e8-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ce6e8-109">Properties</span></span>
| <span data-ttu-id="ce6e8-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ce6e8-110">Property</span></span>     | <span data-ttu-id="ce6e8-111">Typ</span><span class="sxs-lookup"><span data-stu-id="ce6e8-111">Type</span></span>   |<span data-ttu-id="ce6e8-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ce6e8-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce6e8-113">attendee</span><span class="sxs-lookup"><span data-stu-id="ce6e8-113">attendee</span></span>|[<span data-ttu-id="ce6e8-114">AttendeeBase</span><span class="sxs-lookup"><span data-stu-id="ce6e8-114">AttendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="ce6e8-115">Der Typ des Teilnehmers. Unterschieden wird zwischen Personen und Ressourcen. Bei Personen wird zusätzlich differenziert zwischen erforderlichen und optionalen Teilnehmern.</span><span class="sxs-lookup"><span data-stu-id="ce6e8-115">The type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="ce6e8-116">availability</span><span class="sxs-lookup"><span data-stu-id="ce6e8-116">availability</span></span>|<span data-ttu-id="ce6e8-117">String</span><span class="sxs-lookup"><span data-stu-id="ce6e8-117">String</span></span>| <span data-ttu-id="ce6e8-p102">Der Verfügbarkeitsstatus des Teilnehmers. Mögliche Werte sind: `free`, `tentative`, `busy`, `oof`, `workingElsewhere` und `unknown`.</span><span class="sxs-lookup"><span data-stu-id="ce6e8-p102">The availability status of the attendee. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->