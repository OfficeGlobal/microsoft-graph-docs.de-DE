---
title: Ressourcentyp „attendeeAvailability“
description: Die Verfügbarkeit eines Teilnehmers.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 396c53b8d03f573c214dcf43a3637cf06f412a33
ms.sourcegitcommit: a90abf5b89dbbdfefb1b7794d1f12c6e2bfb0cda
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/28/2019
ms.locfileid: "30937782"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="dd786-103">Ressourcentyp „attendeeAvailability“</span><span class="sxs-lookup"><span data-stu-id="dd786-103">attendeeAvailability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd786-104">Die Verfügbarkeit eines Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="dd786-104">The availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd786-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="dd786-105">JSON representation</span></span>

<span data-ttu-id="dd786-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="dd786-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="dd786-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dd786-107">Properties</span></span>
| <span data-ttu-id="dd786-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dd786-108">Property</span></span>     | <span data-ttu-id="dd786-109">Typ</span><span class="sxs-lookup"><span data-stu-id="dd786-109">Type</span></span>   |<span data-ttu-id="dd786-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dd786-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd786-111">attendee</span><span class="sxs-lookup"><span data-stu-id="dd786-111">attendee</span></span>|[<span data-ttu-id="dd786-112">attendeeBase</span><span class="sxs-lookup"><span data-stu-id="dd786-112">attendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="dd786-113">Die e-Mail-Adresse und den Typ des Teilnehmers – unabhängig davon, ob es sich um eine Person oder eine Ressource handelt, und ob Sie erforderlich oder optional ist, wenn es sich um eine Person handelt</span><span class="sxs-lookup"><span data-stu-id="dd786-113">The email address and type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="dd786-114">availability</span><span class="sxs-lookup"><span data-stu-id="dd786-114">availability</span></span>|<span data-ttu-id="dd786-115">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="dd786-115">freeBusyStatus</span></span>| <span data-ttu-id="dd786-p101">Der Verfügbarkeitsstatus des Teilnehmers. Mögliche Werte sind: `free`, `tentative`, `busy`, `oof`, `workingElsewhere` und `unknown`.</span><span class="sxs-lookup"><span data-stu-id="dd786-p101">The availability status of the attendee. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attendeeavailability.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->