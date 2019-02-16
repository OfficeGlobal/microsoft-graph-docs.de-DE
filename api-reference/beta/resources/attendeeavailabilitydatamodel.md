---
title: attendeeAvailabilityDataModel-Ressourcentyp
description: Typ und Verfügbarkeit eines Teilnehmers
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 6d7436a640b4aaba0a9b71ef62ee91b3fe0d7cee
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057382"
---
# <a name="attendeeavailabilitydatamodel-resource-type"></a><span data-ttu-id="f8ff3-103">attendeeAvailabilityDataModel-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f8ff3-103">attendeeAvailabilityDataModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8ff3-104">Stellt eine Person oder Ressource und deren Verfügbarkeit für eine Besprechung dar.</span><span class="sxs-lookup"><span data-stu-id="f8ff3-104">Represents a person or resource and their availability for a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f8ff3-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f8ff3-105">JSON representation</span></span>

<span data-ttu-id="f8ff3-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f8ff3-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeAvailabilityDataModel"
}-->

```json
{
  "attendee": {"@odata.type": "microsoft.graph.attendeeDataModel"},
  "availability": "String"
}

```
## <a name="properties"></a><span data-ttu-id="f8ff3-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f8ff3-107">Properties</span></span>
| <span data-ttu-id="f8ff3-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f8ff3-108">Property</span></span>     | <span data-ttu-id="f8ff3-109">Typ</span><span class="sxs-lookup"><span data-stu-id="f8ff3-109">Type</span></span>   |<span data-ttu-id="f8ff3-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8ff3-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f8ff3-111">attendee</span><span class="sxs-lookup"><span data-stu-id="f8ff3-111">attendee</span></span>|[<span data-ttu-id="f8ff3-112">attendeeDataModel</span><span class="sxs-lookup"><span data-stu-id="f8ff3-112">attendeeDataModel</span></span>](attendeedatamodel.md)|<span data-ttu-id="f8ff3-113">Stellt eine Person oder einen Ressourcen Teilnehmer dar und gibt an, ob der Teilnehmer für die Besprechung erforderlich oder optional ist.</span><span class="sxs-lookup"><span data-stu-id="f8ff3-113">Represents a person or resource attendee and whether the attendee is required or optional for the meeting.</span></span>|
|<span data-ttu-id="f8ff3-114">availability</span><span class="sxs-lookup"><span data-stu-id="f8ff3-114">availability</span></span>|<span data-ttu-id="f8ff3-115">availabilityStatus</span><span class="sxs-lookup"><span data-stu-id="f8ff3-115">availabilityStatus</span></span>| <span data-ttu-id="f8ff3-116">Der Verfügbarkeitsstatus des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="f8ff3-116">The availability status of the attendee.</span></span> <span data-ttu-id="f8ff3-117">Die möglichen Werte sind: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="f8ff3-117">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeAvailabilityDataModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attendeeavailabilitydatamodel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->